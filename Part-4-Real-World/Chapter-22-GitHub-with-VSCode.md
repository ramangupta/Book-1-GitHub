# Chapter 22 — Using GitHub with VSCode

Until now, you have used Git through the terminal.

This is powerful.

But professional developers often use Git through their editor.

VSCode has built-in Git support.

This allows you to:

* See changes visually
* Commit with one click
* Push and pull easily
* Manage branches safely
* Avoid typing complex commands

This makes Git easier and faster.

---

# How VSCode Integrates with Git

VSCode automatically detects Git repositories.

When you open a project folder, VSCode shows Git features.

Open your project:

```bash
code .
```

Look at left sidebar.

You will see:

Source Control icon

Click it.

This is your Git control panel.

---

# First-Time Setup (One-Time Step)

Before using Git in VSCode, ensure Git is installed.

Check using terminal:

```bash
git --version
```

VSCode automatically detects Git.

You will see branch name in bottom-left corner.

If not, install Git and restart VSCode.

This setup is required only once.

---

# Understanding the Source Control Panel

The Source Control panel shows:

* Modified files
* New files
* Deleted files
* Branch name
* Commit options

This gives full visibility of your project state.

Example display:

```
Changes

notes.txt
```

This means file was modified.

---

# Step 1 — Make a Change

Open:

notes.txt

Add new line:

```
This change was made using VSCode.
```

Save the file.

VSCode now marks file as changed.

You will see:

M next to filename.

This means Modified.

---

# Step 2 — Stage the File

In Source Control panel, you will see:

notes.txt

Click:

*

This stages the file.

Staging means preparing file for commit.

Equivalent terminal command:

```bash
git add notes.txt
```

---

# Step 3 — Commit the Change

At top of Source Control panel, you will see message box.

Type:

```
Updated notes using VSCode
```

Click:

Commit button

This saves the commit.

Equivalent terminal command:

```bash
git commit -m "Updated notes using VSCode"
```

---

# Step 4 — Push to GitHub

Click:

Sync Changes

or

Push button

VSCode uploads your changes.

Equivalent terminal command:

```bash
git push
```

Your GitHub repository is now updated.

---

# Signing into GitHub in VSCode

VSCode allows direct GitHub integration.

Click Account icon (bottom-left).

Click:

```
Sign in to GitHub
```

Authorize VSCode.

This allows:

* Push without terminal
* Pull without terminal
* Create pull requests directly

VSCode becomes fully connected to GitHub.

---

# Step 5 — Switch Branch Using VSCode

Look at bottom-left corner.

You will see:

main

Click it.

VSCode shows branch list.

Select another branch.

VSCode switches branch.

Equivalent terminal command:

```bash
git checkout branch-name
```

---

# Step 6 — Create New Branch Using VSCode

Click branch name (bottom-left).

Click:

Create new branch

Enter name:

```
new-feature
```

Press Enter.

VSCode creates and switches branch.

Equivalent terminal command:

```bash
git checkout -b new-feature
```

---

# Step 7 — View File Changes Visually

Click modified file.

VSCode shows:

* Old version
* New version
* Highlighted differences

This is called diff view.

This helps you see exactly what changed.

This is safer than guessing.

---

# Why Professionals Use VSCode for Git

Advantages:

* Visual interface
* Fewer mistakes
* Faster workflow
* Easy branch management
* Clear change tracking

Terminal is still useful.

But VSCode makes Git easier.

Professionals use both.

---

# Professional Workflow Using VSCode

Typical workflow:

1. Open project
2. Create branch
3. Make changes
4. Stage files
5. Commit
6. Push
7. Create pull request

All possible inside VSCode.

---

# Summary

You learned:

* How VSCode integrates with Git
* How to stage and commit visually
* How to push changes
* How to switch branches
* How to create branches

You can now use Git with or without the terminal.

You are working like a professional developer.
