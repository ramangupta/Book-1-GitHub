# Chapter 18 — Git Stash (Temporarily Save Work)

Sometimes you may be working on something that is not finished.

You may have partially completed changes.

But suddenly, you need to switch branches.

Or you need to pull new changes.

Git will not allow branch switching if your working files have uncommitted changes.

You need a safe place to temporarily save your work.

Git provides a solution.

This solution is called `git stash`.

---

## What is Git Stash

`git stash` temporarily saves your uncommitted changes.

It removes the changes from your working folder.

Your folder becomes clean.

Your saved changes are stored safely inside Git.

You can restore them later.

This allows you to switch branches safely.

---

## Understanding the Situation

Imagine you are editing:

```
notes.txt
```

You have made changes.

But you have not committed yet.

Now you need to switch to another branch:

```
git checkout another-branch
```

Git will prevent this.

Because your changes are unfinished.

This is where git stash helps.

---

## Saving Changes Using Stash

Run:

```
git stash
```

Git will:

* Save your changes
* Remove changes from working folder
* Restore folder to last commit state

Your work is safe.

---

## What Happens After Stash

Before stash:

```
notes.txt (modified)
```

After stash:

```
notes.txt (clean)
```

Your changes are saved internally.

Your working folder is clean.

---

## Viewing Stashed Changes

Run:

```
git stash list
```

Output example:

```
stash@{0}: WIP on main
stash@{1}: WIP on feature
```

This shows saved stashes.

---

## Restoring Stashed Changes

To restore most recent stash:

```
git stash pop
```

Git restores your changes.

Your files return to modified state.

---

## Difference Between Pop and Apply

Command:

```
git stash pop
```

Restores changes and removes stash.

Command:

```
git stash apply
```

Restores changes but keeps stash saved.

Pop removes stash.

Apply keeps stash.

---

## Real-World Example

You are working on a feature.

You suddenly need to fix a bug on another branch.

Run:

```
git stash
git checkout main
```

Fix the bug.

Then return:

```
git checkout feature-branch
git stash pop
```

Your unfinished work returns.

Nothing is lost.

---

## Why Professionals Use Git Stash

It allows temporary work storage.

It allows safe branch switching.

It prevents unfinished commits.

It improves workflow flexibility.

It is used daily in real-world development.

---

## Git Stash is Safe

Git stash does not delete your work.

It stores it safely.

You can restore it anytime.

This gives you flexibility and safety.

---

## What You Learned

You learned:

* What git stash is
* How to temporarily save changes
* How to restore stashed changes
* How professionals manage unfinished work

This is an essential real-world Git skill.

It allows flexible and safe development.
