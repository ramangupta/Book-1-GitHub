# Chapter 10 — Fixing Mistakes

Mistakes are normal in software development.

Git makes mistakes safe.

You can fix errors, undo changes, and restore previous versions at any time.

This is one of Git’s most powerful features.

You are never trapped.

---

# Types of Mistakes

There are four common mistake types:

1. Modified file, but not committed
2. Added file, but not committed
3. Committed mistake
4. Want to restore older version

Git can fix all of them.

---

# Case 1 — Modified File, Not Committed

You edited a file:

```bash
code notes.txt
```

Added wrong content.

But you did NOT run git add or git commit.

Check status:

```bash
git status
```

Output:

```
modified: notes.txt
```

To discard changes:

```bash
git checkout -- notes.txt
```

File returns to last committed version.

Mistake is gone.

---

# Case 2 — File Added, But Not Committed

You ran:

```bash
git add notes.txt
```

But want to undo.

Run:

```bash
git reset notes.txt
```

This removes file from staging area.

File remains unchanged.

Only staging is undone.

---

# Case 3 — Wrong Commit Message

You committed:

```bash
git commit -m "Wrong message"
```

Fix it:

```bash
git commit --amend -m "Correct message"
```

Git replaces the commit message.

No code is lost.

---

# Case 4 — Committed Wrong Changes

You committed bad code.

View commits:

```bash
git log
```

Output:

```
commit a1b2c3d
commit e4f5g6h
commit i7j8k9l
```

Each commit has unique ID.

Restore previous version:

```bash
git checkout a1b2c3d
```

Project returns to that state.

You can recover anything.

---

# Case 5 — Undo Last Commit (Keep File Changes)

Run:

```bash
git reset --soft HEAD~1
```

Result:

Last commit removed.

File changes remain.

You can recommit correctly.

---

# Case 6 — Undo Last Commit Completely

Run:

```bash
git reset --hard HEAD~1
```

Result:

Last commit removed.

File changes also removed.

Warning: This permanently deletes changes.

Use carefully.

---

# Understanding HEAD

HEAD means current commit.

HEAD~1 means previous commit.

HEAD~2 means two commits before.

Example:

```
A → B → C → D (HEAD)
```

HEAD~1 → C
HEAD~2 → B

Git moves back safely.

---

# View What Changed

Run:

```bash
git diff
```

Shows exact changes.

This helps identify mistakes.

---

# Safe Recovery Principle

Git stores complete history.

Nothing is truly lost unless force deleted.

This makes Git extremely safe.

---

# Professional Reality

Developers fix mistakes daily.

Git allows:

* Undo errors
* Restore files
* Recover old versions
* Experiment safely

Without Git, mistakes can destroy projects.

With Git, mistakes are harmless.

---

# Summary

You learned how to:

Discard file changes:

```bash
git checkout -- file.txt
```

Unstage file:

```bash
git reset file.txt
```

Fix commit message:

```bash
git commit --amend
```

Undo last commit safely:

```bash
git reset --soft HEAD~1
```

Undo last commit permanently:

```bash
git reset --hard HEAD~1
```

View commit history:

```bash
git log
```

---

# Result

You now have full control over mistakes.

You can safely experiment without fear.

This is why Git is trusted worldwide.
