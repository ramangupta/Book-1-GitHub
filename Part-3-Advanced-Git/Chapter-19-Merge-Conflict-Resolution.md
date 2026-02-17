# Chapter 19 — Merge Conflicts and Resolution

Git allows multiple branches.

Different branches may modify the same file.

When Git tries to merge such branches, it may not know which version is correct.

This situation is called a merge conflict.

Merge conflicts are normal.

Every professional developer encounters them.

Git provides tools to resolve them safely.

---

## What is a Merge Conflict

A merge conflict happens when:

Two branches modify the same part of the same file.

Git cannot automatically decide which change to keep.

Git stops the merge.

It asks you to resolve the conflict manually.

This ensures nothing is lost.

---

## Understanding with an Example

Imagine you have this file:

```
notes.txt
```

Content in main branch:

```
Git is easy.
```

Now in another branch, you change it to:

```
Git is powerful.
```

At the same time, main branch changes it to:

```
Git is fast.
```

Now Git sees two different changes.

Git cannot choose automatically.

This creates a merge conflict.

---

## What Happens During Conflict

When you merge:

```
git merge feature-branch
```

Git shows:

```
CONFLICT (content): Merge conflict in notes.txt
Automatic merge failed.
```

Git stops merging.

It waits for you to resolve the conflict.

---

## How Conflict Appears in File

Open the file.

You will see:

```
<<<<<<< HEAD
Git is fast.
=======
Git is powerful.
>>>>>>> feature-branch
```

These are conflict markers.

They show both versions.

---

## Understanding Conflict Markers

```
<<<<<<< HEAD
```

This is current branch version.

```
=======
```

Separator between versions.

```
>>>>>>> feature-branch
```

This is incoming branch version.

Git is asking you to choose.

---

## How to Resolve Conflict

Edit the file manually.

Choose the correct version.

Example resolved file:

```
Git is fast and powerful.
```

Remove conflict markers.

Save the file.

---

## Mark Conflict as Resolved

After fixing the file, run:

```
git add notes.txt
```

Then complete merge:

```
git commit -m "Resolved merge conflict"
```

Conflict is now resolved.

Merge is complete.

---

## Visual Understanding

Before merge:

```
        A
       / \
      B   C
```

After merge:

```
        A
       / \
      B   C
       \ /
        D
```

D is the merged commit.

---

## Why Merge Conflicts Happen

Merge conflicts happen when:

* Same file is modified in multiple branches
* Same lines are modified
* Git cannot decide automatically

This is normal in team environments.

---

## Important Truth

Merge conflicts are not errors.

They are safety mechanisms.

Git prevents automatic overwriting.

Git ensures you control the final result.

This protects your project.

---

## How Professionals Handle Conflicts

Professionals:

* Read both versions carefully
* Choose correct version
* Combine changes when needed
* Test after resolving

Conflict resolution is part of daily development.

---

## How to Reduce Merge Conflicts

You can reduce conflicts by:

* Pulling regularly
* Keeping branches updated
* Making small changes
* Avoiding long-lived branches

This improves workflow.

---

## What You Learned

You learned:

* What merge conflicts are
* Why merge conflicts happen
* How conflict markers work
* How to resolve conflicts safely
* How professionals handle conflicts

You now understand one of the most important real-world Git skills.

You now have full control over merging changes.

You have completed Advanced Git.
