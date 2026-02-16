# Chapter 4 — Making Changes and Updating GitHub

Software projects are never written once.

They evolve.

You will constantly:

* Add new files
* Modify existing files
* Fix mistakes
* Improve features

Git tracks these changes.

GitHub stores them safely online.

In this chapter, you will learn how to update your project.

---

## Step 1 — Modify an Existing File

Open your project folder:

```bash
cd my-first-project
code .
```

Open the file:

```bash
notes.txt
```

Change it from:

```
This is my first Git project.
```

to:

```
This is my first Git project.

Git is tracking my changes.
```

Save the file.

---

## Step 2 — Check What Changed

Run:

```bash
git status
```

You will see:

```bash
modified: notes.txt
```

This means Git detected changes.

But Git has not saved them yet.

---

## Step 3 — Add Changes to Git

Run:

```bash
git add notes.txt
```

This prepares the file for saving.

Check status again:

```bash
git status
```

You will see:

```bash
Changes to be committed:
modified: notes.txt
```

---

## Step 4 — Commit the Changes

Run:

```bash
git commit -m "Updated notes.txt with new line"
```

Git will respond:

```bash
1 file changed
```

Git has now saved a new version.

---

## Step 5 — Upload Changes to GitHub

Run:

```bash
git push
```

Git will upload your changes to GitHub.

Output will look like:

```bash
To https://github.com/yourusername/my-first-project.git
   7f3a8c2..9a5b1d3  main -> main
```

Your GitHub repository is now updated.

---

## Step 6 — Verify on GitHub

Go to your repository:

```
https://github.com/yourusername/my-first-project
```

Click:

```
notes.txt
```

You will see the updated content.

Your changes are now online.

---

## Important Concept — Git Workflow

Every update follows this cycle:

```bash
Edit file
git add
git commit
git push
```

This is the core Git workflow.

You will use this thousands of times.

---

## Important Concept — Version History

Each commit creates a permanent record.

View history:

```bash
git log
```

Example:

```bash
commit 9a5b1d3 Updated notes.txt with new line
commit 7f3a8c2 Initial commit
```

You can always go back to previous versions.

This makes Git extremely powerful.

---

## Summary

You have now learned how to:

* Modify files
* Track changes
* Commit changes
* Upload updates to GitHub
* Maintain version history

You are now managing a real software project.

This is exactly how professional developers work.
