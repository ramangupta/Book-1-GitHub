# Chapter 9 — Merging Changes (Combining Branch Work Safely)

In the previous chapter, you learned how to create branches.

Branches allow you to work safely without affecting the main project.

You can add features, fix bugs, and experiment in isolation.

But eventually, your work must become part of the main project.

This is called merging.

---

## What is Merging

Merging means combining changes from one branch into another branch.

Most commonly, you merge a feature branch into the main branch.

This allows your new work to become part of the main project.

Think of it like this:

main branch = stable project
feature branch = new work

Merging combines the new work into the stable project.

---

## Why Merging is Needed

When you create a branch, your changes stay in that branch.

The main branch does not see those changes.

This is intentional.

Branches protect the main project from unfinished or experimental work.

When your work is complete and safe, you merge it into main.

This updates the main project safely.

---

## Example Scenario

You create a branch:

```bash
git checkout -b new-feature
```

You create a file:

```bash
nano feature.txt
```

Add content:

```
This is a new feature
```

Save the file.

Commit the change:

```bash
git add .
git commit -m "Added new feature"
```

This change exists only in the branch.

Main branch remains unchanged.

---

## Switch Back to Main Branch

Before merging, switch to the main branch:

```bash
git checkout main
```

You must always switch to the branch that will receive the changes.

In this case, main will receive the changes.

---

## Merge the Branch

Run the merge command:

```bash
git merge new-feature
```

Example output:

```bash
Updating a1b2c3d..e4f5g6h
Fast-forward
 feature.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt
```

This means the merge was successful.

The changes from new-feature are now part of main.

---

## Verify the Merge

Check files:

```bash
ls
```

You will see:

```
feature.txt
```

The file from the branch is now in main.

The merge is complete.

---

## What Happened Internally

Before merge:

main branch:

```
project files
```

feature branch:

```
project files
feature.txt
```

After merge:

main branch:

```
project files
feature.txt
```

The main branch now includes the new feature.

---

## Branch Still Exists

After merging, the branch still exists.

Check branches:

```bash
git branch
```

Output:

```bash
* main
  new-feature
```

The branch is still available.

You can delete it if no longer needed.

---

## Delete the Branch (Optional)

Run:

```bash
git branch -d new-feature
```

This deletes the branch.

Your changes remain in main.

Deleting the branch does not remove the merged work.

---

## Professional Workflow Summary

Professional developers follow this workflow:

1. Create branch
2. Work in branch
3. Commit changes
4. Merge branch into main
5. Delete branch

This keeps the project safe and organized.

Main branch remains stable.

Branches allow safe development.

Merging safely integrates completed work.

---

## Important Rule

Never merge unfinished or broken work into main.

Only merge when your changes are complete and safe.

This protects the stability of the project.

---

## Commands Learned

Create branch:

```bash
git checkout -b new-feature
```

Switch branch:

```bash
git checkout main
```

Merge branch:

```bash
git merge new-feature
```

Delete branch:

```bash
git branch -d new-feature
```

---

## What You Achieved

You learned how to safely combine branch work into the main project.

You can now:

* Create isolated branches
* Work safely
* Merge completed work
* Maintain project stability

This is the core of professional Git workflow.

Next, you will learn about merge conflicts and how to resolve them.
