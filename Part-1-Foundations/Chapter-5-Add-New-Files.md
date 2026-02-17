# Chapter 5 — Creating and Uploading New Files

Until now, you modified an existing file.

Now you will learn how to create completely new files and upload them to GitHub.

This is how real projects grow.

---

## Step 1 — Create a New File

Inside your project folder, run:

```bash
touch ideas.txt
```

This creates a new empty file.

Open in VSCode:

```bash
code .
```

Open:

```
ideas.txt
```

Write:

```
Future project ideas:

- Build a website
- Build an AI tool
- Learn backend development
```

Save the file.

---

## Step 2 — Check Git Status

Run:

```bash
git status
```

Output:

```bash
Untracked files:
ideas.txt
```

Untracked means Git sees the file but is not tracking it yet. Untracked files are files in your project folder that Git has noticed exists but hasn’t started tracking yet.

To track them, we use git add.

File States in Git:

File Name       State
---------       -----
example.txt     untracked   → just created, not yet staged
example.txt     staged      → added with 'git add', ready to commit
example.txt     committed   → saved in Git history

![Git Stages](../images/Git_3_stages.png)

---

## Step 3 — Add the New File (Staging)

Run:

```bash
git add ideas.txt
```
Staging means telling Git, “Include this file in the next commit.”
Until you commit, the file isn’t saved in history.

Now check status:

```bash
git status
```

Output:

```bash
Changes to be committed:
new file: ideas.txt
```

Git is now ready to save it.

---

## Step 4 — Commit the New File

Run:

```bash
git commit -m "Added ideas.txt with project ideas"
```

Git saves the file permanently.

---

## Step 5 — Upload to GitHub

Run:

```bash
git push
```

Git uploads the new file.

---

## Step 6 — Verify on GitHub

Go to:

```
https://github.com/yourusername/my-first-project
```

You will see:

```
notes.txt
ideas.txt
```

Your project has grown.

---

## Important Concept — Git Tracks Entire Projects

Git does not track only one file.

It tracks:

* All files
* All changes
* Complete history

This makes Git a complete project tracking system.

---

## Important Concept — Multiple File Workflow

Whenever you create or modify files:

```bash
git add filename
git commit -m "message"
git push
```

Or add all files at once:

```bash
git add .
git commit -m "message"
git push
```

The dot (.) means:

Add everything.

---

## Summary

You have now learned how to:

* Create new files
* Track new files
* Commit new files
* Upload new files to GitHub

Your project can now grow infinitely.

This is how real software is built.
