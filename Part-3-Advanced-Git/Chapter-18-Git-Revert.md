# Chapter 18 — Git Revert (Safe Undo for Shared Projects)

In the previous chapter, you learned about `git reset`.

Git reset removes commits from history.

This works well for local commits.

But in professional environments, commits are often shared.

They are pushed to GitHub.

Other developers may already be using those commits.

Removing such commits can cause serious problems.

Git provides a safer solution.

This solution is called `git revert`.

---

## What is Git Revert

`git revert` safely undoes a commit.

It does not delete the commit.

Instead, it creates a new commit that reverses the changes.

This keeps history safe and complete.

This is the professional way to undo changes.

---

## Understanding the Concept

Imagine your commit history looks like this:

```
Commit A → Commit B → Commit C
```

Commit C contains a mistake.

You want to undo it.

Using revert creates:

```
Commit A → Commit B → Commit C → Commit D
```

Commit D reverses Commit C.

Commit C still exists.

History remains safe.

---

## Why This is Important

In shared repositories:

* Other developers depend on commit history
* Removing commits can break their work
* Reset can create conflicts

Revert avoids this problem.

It preserves history.

It maintains safety.

---

## How to Use Git Revert

First, view commit history:

```
git log
```

Output example:

```
a1b2c3 Commit C
d4e5f6 Commit B
g7h8i9 Commit A
```

To revert Commit C:

```
git revert a1b2c3
```

Git creates a new commit.

This commit undoes Commit C.

---

## What Happens After Revert

Before revert:

```
Commit A → Commit B → Commit C
```

After revert:

```
Commit A → Commit B → Commit C → Revert Commit
```

The mistake is undone safely.

History remains intact.

---

## Real Example

You committed incorrect content:

```
git commit -m "Added wrong configuration"
```

You already pushed it to GitHub.

Now you fix it safely:

```
git revert HEAD
```

Git creates a new commit.

The incorrect changes are undone.

---

## Difference Between Reset and Revert

Git Reset:

* Removes commits
* Changes history
* Unsafe for shared repositories

Git Revert:

* Keeps commits
* Adds a new undo commit
* Safe for shared repositories

Professionals prefer revert for shared work.

---

## When to Use Git Revert

Use revert when:

* You already pushed commits
* You are working with a team
* You want safe undo
* You want to preserve history

This is the safest undo method.

---

## Why Professionals Use Git Revert

It prevents breaking shared history.

It keeps project stable.

It allows safe correction of mistakes.

It maintains complete commit records.

This makes Git reliable for teams.

---

## What You Learned

You learned:

* What git revert is
* How revert safely undoes commits
* Why revert is safer than reset for shared projects
* How professionals undo mistakes safely

You now understand safe history correction.

This is an essential professional Git skill.
