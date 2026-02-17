# Chapter 17 — Git Reset (Undo Commits)

Sometimes you may commit something by mistake.

You may:

* Commit too early
* Commit incorrect changes
* Commit unwanted files
* Want to modify a previous commit

Git provides a powerful command to handle this.

This command is called `git reset`.

---

## What is Git Reset

`git reset` allows you to undo commits.

It moves the current branch back to a previous commit.

This gives you control over your project history.

It allows you to correct mistakes safely.

---

## Understanding Commits as a Timeline

Imagine your commit history looks like this:

```
Commit A → Commit B → Commit C
```

Your current position is at Commit C.

Now you want to go back to Commit B.

Git reset allows this.

---

## Basic Reset Command

```
git reset HEAD~1
```

This moves Git back by one commit.

HEAD represents the current commit.

HEAD~1 means one commit before the current commit.

---

## What Happens After Reset

Before reset:

```
Commit A → Commit B → Commit C (Current)
```

After reset:

```
Commit A → Commit B (Current)
```

Commit C is removed from commit history.

But its file changes remain in your working folder.

You can modify them and commit again.

---

## Types of Git Reset

Git reset has three modes:

* Soft reset
* Mixed reset
* Hard reset

Each behaves differently.

---

## Soft Reset (Safest Reset)

Command:

```
git reset --soft HEAD~1
```

Effect:

* Removes the commit
* Keeps file changes
* Keeps files staged

This allows you to recommit easily.

---

## Mixed Reset (Default Reset)

Command:

```
git reset HEAD~1
```

Effect:

* Removes the commit
* Keeps file changes
* Removes staging

Files must be staged again before committing.

This is the default behavior.

---

## Hard Reset (Dangerous Reset)

Command:

```
git reset --hard HEAD~1
```

Effect:

* Removes the commit
* Removes file changes
* Deletes all uncommitted work

This cannot be easily undone.

Use hard reset carefully.

---

## Visual Example

Before hard reset:

```
Commit A → Commit B → Commit C
```

After hard reset:

```
Commit A → Commit B
```

Commit C and its changes are completely removed.

---

## When to Use Git Reset

Use git reset when:

* You committed by mistake
* You want to modify a commit
* You want to remove unwanted commits

It gives you precise control.

---

## Important Warning

Do not use reset on commits that are already pushed to GitHub.

Reset changes history.

This can cause problems for teams.

Reset is safest when used on local commits.

---

## Real-World Example

You accidentally commit a temporary file:

```
git add temp.txt
git commit -m "Temporary file"
```

You realize this was a mistake.

Run:

```
git reset HEAD~1
```

The commit is removed.

You can now fix the mistake.

---

## Why Professionals Use Git Reset

It allows correction of commit mistakes.

It keeps project history clean.

It gives complete control over commits.

It is an essential advanced Git skill.

---

## What You Learned

You learned:

* What git reset is
* How to undo commits
* Difference between soft, mixed, and hard reset
* How Git controls commit history

You now have powerful control over your commits.

You are learning how professionals manage Git history.
