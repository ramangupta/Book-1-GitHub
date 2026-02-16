# Chapter 7 — Pulling Latest Changes from GitHub

Your project exists in two places:

* Local repository (your computer)
* Remote repository (GitHub)

Sometimes, the remote repository gets new changes.

Example:

* You edited files from another computer
* Someone else updated the project
* You edited directly on GitHub

Your local copy becomes outdated.

You need to update it.

This is called pulling.

---

## Important Concept — Pull

Pull = Download latest changes from GitHub into your local repository.

It synchronizes your project.

Direction:

Remote → Local

---

## Step 1 — Go to Your Project Folder

Open terminal.

Run:

```bash
cd my-first-project
```

---

## Step 2 — Pull Latest Changes

Run:

```bash
git pull
```

Output example:

```bash
Updating 7f3a8c2..9d4b21a
1 file changed
```

Git downloads and updates your files.

---

## Step 3 — Verify Files

Check files:

```bash
ls
```

Open files in VSCode:

```bash
code .
```

You will see the latest version.

---

## Real World Example

Computer A:

You add a new file:

```bash
touch newfile.txt
git add .
git commit -m "Added new file"
git push
```

Computer B:

Run:

```bash
git pull
```

newfile.txt appears.

This keeps both machines synchronized.

---

## Important Concept — Daily Workflow

Real developers follow this pattern:

Start work:

```bash
git pull
```

Do work:

(edit files)

Save work:

```bash
git add .
git commit -m "message"
git push
```

Repeat daily.

---

## Important Concept — Push vs Pull

Push:

Local → GitHub

Pull:

GitHub → Local

Both keep your project synchronized.

---

## Step 4 — Check Repository Status

Run:

```bash
git status
```

Output:

```bash
On branch main
nothing to commit, working tree clean
```

This means everything is synchronized.

---

## Summary

You have now learned:

* How to download latest changes
* How to synchronize repositories
* How developers collaborate safely
* Full Git workflow

You now know the complete Git cycle:

clone → edit → add → commit → push → pull

You are now operating like a real software developer.
