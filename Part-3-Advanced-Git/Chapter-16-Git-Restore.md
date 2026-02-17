# Chapter 16 — Git Restore (Undo File Changes Safely)

Mistakes are a normal part of development.

You may accidentally:

* Modify a file incorrectly
* Delete important content
* Change something you did not intend to change

Git provides a safe way to undo such changes.

This command is called `git restore`.

---

## What is Git Restore

`git restore` allows you to undo changes in files.

It restores files to their previous state.

It is a safe and controlled recovery tool.

It does not damage your repository.

It simply brings back the last committed version of a file.

---

## Understanding the Situation

Imagine your file contains:

```
notes.txt
```

Content:

```
Git is easy to learn.
```

You commit this file.

Now you accidentally change it to:

```
Git is very difficult.
```

This change is not yet committed.

You want to undo it.

This is where `git restore` is used.

---

## Checking File Status

Run:

```
git status
```

Output may show:

```
modified: notes.txt
```

This means the file was changed.

Git has detected the modification.

---

## Restoring the File

Run:

```
git restore notes.txt
```

Git will restore the file.

The incorrect change will be removed.

The file returns to the last committed version.

---

## What Actually Happened

Before restore:

```
Git is very difficult.
```

After restore:

```
Git is easy to learn.
```

Git recovered the previous version safely.

---

## Important Safety Feature

`git restore` only affects uncommitted changes.

It does not affect committed history.

Your commits remain safe.

This makes `git restore` a safe command.

---

## Restoring Multiple Files

You can restore multiple files:

```
git restore file1.txt file2.txt
```

Git restores both files.

---

## Restoring All Files

You can restore all modified files:

```
git restore .
```

The dot means current folder.

Git restores all modified files.

---

## Restoring Staged Files

Sometimes you add a file using:

```
git add notes.txt
```

This moves the file to staging area.

To remove it from staging area:

```
git restore --staged notes.txt
```

This removes it from staging.

The file remains unchanged.

---

## Understanding the Difference

Command:

```
git restore notes.txt
```

Effect:

Restores file content

Command:

```
git restore --staged notes.txt
```

Effect:

Removes file from staging area

Both are safe operations.

---

## Real-World Use Case

You accidentally modify 10 files.

Only 2 files should be changed.

You can restore the other 8 files safely.

Without affecting your commits.

This saves time and prevents mistakes.

---

## Why Professionals Use Git Restore

It allows safe recovery.

It prevents accidental commits.

It helps maintain clean history.

It provides confidence while working.

Professional developers use this frequently.

---

## What You Learned

You learned:

* What `git restore` is
* How to undo file changes
* How to restore staged files
* How Git safely recovers files

This is an essential recovery tool.

It gives you safety while working.

You now have greater control over your project.
