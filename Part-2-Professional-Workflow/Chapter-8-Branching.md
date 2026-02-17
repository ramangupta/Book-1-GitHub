# Chapter 8 — Branching (Working Without Breaking Main Code)

---

# The Problem Branching Solves

Imagine your project is working perfectly.

It runs.
It is stable.
It is safe.

Now you want to add a new feature.

But what if you break something?

Your main project will stop working.

This is dangerous.

Professional developers never experiment directly on the main code.

They use branches.

---

# What is a Branch

A branch is a separate version of your project.

It allows you to work safely without affecting the main version.

Think of it like this:

Main branch = stable version
New branch = experiment version

Your main branch stays safe.

---

# Visual Understanding

Main branch:

Version 1 → Version 2 → Version 3

New branch:

Version 3 → Experiment 1 → Experiment 2

Main branch is untouched.

![Git Branching Concept](images/human_git_branch.png)


---

# Real World Analogy

Think of your project like a book.

Main branch = published book
Branch = draft copy

You edit the draft.

Your published book stays safe.

---

# Default Branch Name

The default branch is called:

main

This is the primary version of your project.

---

# Check Your Current Branch

Open Terminal and run:

```bash
git branch
```

Output example:

```bash
* main
```

The star (*) shows your current branch.

You are currently on main.

---

# Create a New Branch

Command:

```bash
git branch new-feature
```

This creates a branch named new-feature.

Your project is still on main.

---

# Switch to the New Branch

Command:

```bash
git checkout new-feature
```

Now you are working inside new-feature branch.

Check again:

```bash
git branch
```

Output:

```bash
main
* new-feature
```

Now new-feature is active.

---

# Shortcut Command (Create and Switch)

Instead of two commands, use one:

```bash
git checkout -b new-feature
```

This creates and switches instantly.

---

# Make Changes in Branch

Now create or edit files.

Example:

```bash
nano test.txt
```

Add text:

This is a branch test

Save file.

---

# Commit Changes in Branch

```bash
git add .
git commit -m "Testing branch"
```

This commit exists only in new-feature branch.

Main branch is untouched.

---

# Switch Back to Main Branch

```bash
git checkout main
```

Your branch changes disappear.

Because they belong to new-feature branch.

This is correct behavior.

---

# Why Branching is Powerful

Branching allows you to:

Add features safely
Fix bugs safely
Experiment safely
Work in teams safely

Without breaking main project.

---

# Professional Rule

Never work directly on main branch.

Always create a branch.

---

# Summary

Branch = safe workspace

Main branch = stable version
Branch = experimental version

Commands learned:

Check branch:

```bash
git branch
```

Create branch:

```bash
git branch branch-name
```

Switch branch:

```bash
git checkout branch-name
```

Create and switch:

```bash
git checkout -b branch-name
```

---

# What You Achieved

You learned how professionals work safely.

You can now experiment without fear.

Next chapter:

Merging Changes.
