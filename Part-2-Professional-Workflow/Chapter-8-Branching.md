# Chapter 8 — Branching (Working Without Breaking Main Code)

In professional software development, stability is critical.

Your main project must always remain safe, functional, and reliable.

But development requires change.

You will add features.
You will fix bugs.
You will experiment.

What happens if a change breaks the project?

The main version will stop working.

This is dangerous.

Professional developers never experiment directly on the main code.

They use branches.

---

## The Problem Branching Solves

Imagine your project is working perfectly.

It runs.
It is stable.
It is safe.

Now you want to add a new feature.

If you modify the main code directly and something breaks, the entire project becomes unstable.

This affects everyone using the project.

Professional projects must always keep the main version safe.

Branching solves this problem.

---

## What is a Branch

A branch is a separate version of your project.

It allows you to work safely without affecting the main version.

Think of it like this:

Main branch = stable version
Branch = experimental version

Your main branch remains untouched while you work in a branch.

Branches allow developers to work independently without affecting the main codebase, making development safer and more organized. 

---

## Visual Understanding


Conceptually:

```
main branch:
Version 1 → Version 2 → Version 3

new-feature branch:
Version 3 → Experiment 1 → Experiment 2
```

The main branch continues safely.

Your experimental work happens separately.

---

## Real-World Analogy

Think of your project like a published book.

Main branch = published book
Branch = draft copy

You edit the draft.

Your published book remains unchanged.

Only when the draft is ready do you update the published version.

---

## Default Branch Name

The default branch is called:

```
main
```

This is the primary and stable version of your project.

All professional workflows protect the main branch.

---

## Check Your Current Branch

Open Terminal and run:

```bash
git branch
```

Example output:

```bash
* main
```

The star (*) shows your current branch.

You are currently working on the main branch.

---

## Create a New Branch

Command:

```bash
git branch new-feature
```

This creates a new branch called:

```
new-feature
```

Your project is still on main.

You have only created the branch.

You have not switched to it yet.

---

## Switch to the New Branch

Command:

```bash
git checkout new-feature
```

Now you are working inside the new branch.

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

## Shortcut Command (Create and Switch Instantly)

Instead of two commands, you can use one:

```bash
git checkout -b new-feature
```

This command:

* Creates the branch
* Switches to the branch

in one step.

This is commonly used by professional developers.

---

## Make Changes in the Branch

Now create or modify files.

Example:

```bash
nano test.txt
```

Add text:

```
This is a branch test
```

Save the file.

---

## Commit Changes in the Branch

```bash
git add .
git commit -m "Testing branch"
```

This commit exists only in the branch.

The main branch remains unchanged.

Your main project is still safe.

---

## Switch Back to Main Branch

Command:

```bash
git checkout main
```

You will notice your branch changes are not visible.

This is correct behavior.

Those changes belong to the branch, not main.

This isolation is what makes branching powerful.

---

## Why Branching is Powerful

Branching allows you to:

* Add features safely
* Fix bugs safely
* Experiment safely
* Work in teams safely

Without breaking the main project.

Branches isolate development work, allowing multiple changes without affecting the stable version. 

---

## Professional Rule

Professional developers follow this rule:

Never work directly on main.

Always create a branch.

This keeps the project stable and safe.

---

## Summary

Branch = safe workspace
Main branch = stable version
Branch = isolated development environment

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

## What You Achieved

You learned how professional developers work safely.

You can now:

* Create branches
* Work safely
* Protect the main project
* Experiment without risk

Branches are the foundation of professional Git workflow.

Next chapter: Merging Changes.


