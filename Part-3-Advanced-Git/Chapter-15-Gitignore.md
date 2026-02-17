# Chapter 15 — .gitignore (Ignoring Unnecessary Files)

In real-world projects, not every file should be tracked by Git.

Some files are temporary.

Some files are automatically generated.

Some files contain private or sensitive information.

Tracking such files creates problems.

Git provides a solution.

This solution is called `.gitignore`.

---

## What is .gitignore

`.gitignore` is a special file.

It tells Git which files to ignore.

Ignored files are not tracked.

Ignored files are not committed.

Ignored files are not pushed to GitHub.

Git simply leaves them alone.

This keeps your repository clean and safe.

---

## Why Ignoring Files is Important

Many files do not belong in version control.

Examples include:

* Temporary files
* Log files
* Build output files
* System files
* Dependency folders
* Secret configuration files

These files:

* Change frequently
* Increase repository size
* Create unnecessary clutter
* May expose sensitive information

Professional developers always use `.gitignore`.

---

## Real Example

Imagine your project folder contains:

```
notes_app/
notes.txt
debug.log
temp.txt
```

You only want to track:

```
notes.txt
```

You do not want:

```
debug.log
temp.txt
```

to be tracked.

`.gitignore` solves this.

---

## Creating .gitignore File

Create a file named:

```
.gitignore
```

Important:

The file name starts with a dot.

This makes it a hidden file.

---

## Example .gitignore Content

Open `.gitignore` and write:

```
*.log
temp.txt
```

This tells Git:

Ignore all `.log` files
Ignore `temp.txt`

---

## What This Means

Git will now ignore:

```
debug.log
temp.txt
```

Git will still track:

```
notes.txt
```

Only important files remain under version control.

---

## Ignoring Entire Folders

You can ignore folders.

Example:

```
node_modules/
```

Git will ignore the entire folder.

This is very common in software projects.

---

## Ignoring System Files

Example:

```
.DS_Store
Thumbs.db
```

These are system-generated files.

They should not be tracked.

---

## How Git Behaves After .gitignore

After creating `.gitignore`:

Run:

```
git status
```

Ignored files will not appear.

Git will behave as if they do not exist.

This keeps your repository clean.

---

## Important Rule

`.gitignore` only affects untracked files.

If a file is already tracked, `.gitignore` will not ignore it automatically.

Git continues tracking it.

To stop tracking, you must remove it manually.

(This will be covered later.)

---

## Real-World Example (.gitignore)

Professional projects often use:

```
node_modules/
.env
*.log
dist/
build/
__pycache__/
```

These files and folders are not needed in version control.

---

## Why Professionals Always Use .gitignore

Without `.gitignore`:

Repository becomes large
Repository becomes messy
Sensitive data may leak
Project becomes harder to manage

With `.gitignore`:

Repository stays clean
Repository stays safe
Project stays professional

---

## What You Learned

You learned:

* What `.gitignore` is
* Why ignoring files is important
* How to create `.gitignore`
* How Git ignores files
* How professionals use `.gitignore`

This is an essential real-world Git skill.

You are now learning how professionals manage repositories.
