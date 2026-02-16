# Chapter 11 — Viewing File History

Every change in Git is recorded permanently.

This means you can see:

* Who changed a file
* When it was changed
* What exactly was changed
* Why it was changed

This is called **history tracking**.

This feature makes debugging and auditing possible.

---

# View All Commits

Run:

```bash
git log
```

Example output:

```
commit a1b2c3d4e5f6
Author: Ian Cooper
Date: Tue Jan 10 10:30:21 2026

Added login feature

commit f7g8h9i0j1k2
Author: Ian Cooper
Date: Mon Jan 9 09:12:11 2026

Initial commit
```

Each commit contains:

* Commit ID
* Author
* Date
* Message

This is your project timeline.

---

# Simplified View (Professional Usage)

Run:

```bash
git log --oneline
```

Output:

```
a1b2c3d Added login feature
f7g8h9i Initial commit
```

This is faster and easier to read.

Professional developers use this often.

---

# View Changes Inside a Commit

Run:

```bash
git show a1b2c3d
```

Git displays:

* Files modified
* Lines added
* Lines removed

You see exactly what changed.

---

# View File History Only

To see history of a specific file:

```bash
git log notes.txt
```

Output shows only commits affecting that file.

This helps track file evolution.

---

# See What Changed Between Commits

Run:

```bash
git diff a1b2c3d f7g8h9i
```

Git shows difference between versions.

This is useful for debugging.

---

# See Who Modified Each Line

Run:

```bash
git blame notes.txt
```

Example output:

```
a1b2c3d Ian Cooper Added login feature
f7g8h9i Ian Cooper Initial commit
```

This shows:

* Who wrote each line
* When it was written

This is critical in team environments.

---

# View Current Changes (Not Yet Committed)

Run:

```bash
git diff
```

Shows changes since last commit.

This helps review before committing.

---

# Visual Timeline Concept

Example timeline:

```
A --- B --- C --- D --- E
```

Each letter is a commit.

Git remembers every step.

You can return to any point.

---

# Why History Tracking is Powerful

Without Git:

* Changes are lost
* Bugs are hard to trace
* No accountability

With Git:

* Every change is recorded
* Bugs can be traced easily
* Full transparency

This makes software reliable.

---

# Professional Reality

In large companies:

Projects may have:

* 10,000+ commits
* Hundreds of developers

Git manages all history safely.

This makes collaboration possible.

---

# Summary

View full history:

```bash
git log
```

View simplified history:

```bash
git log --oneline
```

View commit details:

```bash
git show commit-id
```

View file history:

```bash
git log file.txt
```

Compare versions:

```bash
git diff commit1 commit2
```

See line authors:

```bash
git blame file.txt
```

---

# Result

You can now inspect any change in your project.

You have full visibility and control.

This makes debugging and auditing easy.
