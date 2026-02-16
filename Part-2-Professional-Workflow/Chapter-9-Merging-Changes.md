# Chapter 9 — Merging Changes

Branching allows you to work safely.

But at some point, you want to bring your changes back into the main branch.

This process is called merging.

Merging combines changes from one branch into another.

Most commonly:

new-feature → main

---

## Why Merging is Needed

You created a branch to experiment safely.

Now the feature works correctly.

You want the main project to include this feature.

So you merge the branch into main.

Result:

Main branch gets the new feature.

---

## Visual Understanding

Before merge:

Main branch:

A --- B --- C

New-feature branch:

A --- B --- C --- D --- E

Main does not yet have D and E.

After merge:

Main branch:

A --- B --- C --- D --- E

Both branches now contain the same changes.

---

## Step 1 — Switch to Main Branch

Always merge into the target branch.

In this case, target is main.

Run:

```bash
git checkout main
```

You are now on main branch.

Verify:

```bash
git branch
```

Output:

```
* main
  new-feature
```

---

## Step 2 — Merge the Branch

Run:

```bash
git merge new-feature
```

Git will merge the changes.

Output may look like:

```
Updating a1b2c3d..e4f5g6h
Fast-forward
 notes.txt | 1 +
 1 file changed, 1 insertion(+)
```

Merge is complete.

Main now contains the changes.

---

## Step 3 — Verify the Merge

Open your file:

```bash
code notes.txt
```

You will now see the new feature content.

This confirms merge was successful.

---

## What Happened Internally

Before merge:

main → A → B → C
new-feature → A → B → C → D → E

After merge:

main → A → B → C → D → E

Git moved main forward.

No data was lost.

---

## Delete the Branch (Optional but Recommended)

Once merged, branch is no longer needed.

Delete it:

```bash
git branch -d new-feature
```

Output:

```
Deleted branch new-feature
```

Your repository is now clean.

---

## Important Rule

Always merge into main.

Do NOT merge main into feature branch unless necessary.

Correct workflow:

1. Create branch
2. Make changes
3. Commit changes
4. Switch to main
5. Merge branch into main

---

## Real World Example

You create branch:

login-feature

You build login system.

It works correctly.

You merge:

login-feature → main

Now main has login system.

---

## Professional Workflow Summary

Create branch:

```bash
git checkout -b new-feature
```

Make changes and commit:

```bash
git add .
git commit -m "Added feature"
```

Switch to main:

```bash
git checkout main
```

Merge:

```bash
git merge new-feature
```

Delete branch:

```bash
git branch -d new-feature
```

---

## Result

Your feature is now part of the main project.

Project safely grows without breaking existing code.

This is the foundation of professional software development.
