# Chapter 10 — Fixing Mistakes (Recovering Safely with Git)

Mistakes are a normal part of software development.

Every developer makes mistakes.

You may:

* Modify the wrong file
* Add incorrect content
* Commit too early
* Delete something accidentally

Without version control, mistakes can be dangerous.

You may lose important work permanently.

Git solves this problem.

Git allows you to safely recover from mistakes.

---

## How Git Protects You

Git saves your project as a series of commits.

Each commit is a snapshot of your project at a specific moment.

Think of commits like save points in a game.

You can always go back to a previous save point.

Your work is never truly lost.

This makes Git extremely safe.

---

## View Project History

To see your commit history, run:

```bash
git log
```

Example output:

```bash
commit a1b2c3d4e5f6g7h8i9j0
Author: Your Name
Date: Today

Added new feature
```

Each commit has a unique ID.

This ID allows Git to track every change.

---

## Common Mistake Scenario

Imagine you modify a file incorrectly.

Example:

```bash
nano notes.txt
```

You accidentally delete important content.

You save the file.

This is a mistake.

Git can restore the correct version.

---

## Check Current Status

Run:

```bash
git status
```

Git will show modified files.

This tells you what has changed.

---

## Restore File to Last Committed Version

Command:

```bash
git restore notes.txt
```

This restores the file to its last committed state.

Your mistake is removed.

Your safe version is restored.

---

## If You Already Staged the File

If you used:

```bash
git add notes.txt
```

You can unstage it:

```bash
git restore --staged notes.txt
```

This removes the file from staging.

Your file returns to modified state.

---

## Undo Last Commit (Keep Changes)

If you committed too early, run:

```bash
git reset --soft HEAD~1
```

This removes the last commit.

Your changes remain in the working directory.

You can fix and commit again.

---

## Undo Last Commit (Remove Changes Completely)

If you want to completely remove the last commit and its changes:

```bash
git reset --hard HEAD~1
```

This permanently removes the commit and changes.

Use this carefully.

---

## Important Safety Concept

Git does not delete commits immediately.

Git keeps history safely.

Most mistakes can be recovered.

This makes Git reliable and safe.

Professional developers trust Git because of this protection.

---

## Professional Workflow Protection

Developers use commits regularly.

Each commit creates a recovery point.

If something breaks, developers restore a previous commit.

This prevents permanent damage.

Git allows safe experimentation.

---

## Commands Learned

View history:

```bash
git log
```

Restore file:

```bash
git restore filename
```

Unstage file:

```bash
git restore --staged filename
```

Undo last commit (keep changes):

```bash
git reset --soft HEAD~1
```

Undo last commit (remove changes):

```bash
git reset --hard HEAD~1
```

---

## What You Achieved

You learned how to safely recover from mistakes.

You can now:

* Restore files
* Undo commits
* Recover from errors
* Protect your project

This gives you complete control over your project.

Mistakes are no longer dangerous.

Git makes development safe.
