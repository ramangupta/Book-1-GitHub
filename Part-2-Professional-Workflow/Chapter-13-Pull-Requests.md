# Chapter 13 — Pull Requests (Professional Collaboration)

Pull Requests are one of the most important features of GitHub.

They allow developers to safely propose changes to a project.

Pull Requests are used in:

* Software companies
* Open source projects
* Professional teams
* Personal projects

This is how modern software is built.

---

# What is a Pull Request?

A Pull Request (PR) is a request to merge changes from one branch into another branch.

Usually:

```
new-feature → main
```

It means:

"I made changes in my branch. Please review and merge them into main."

Pull Requests allow review before merging.

This keeps the main branch safe.

---

# Why Pull Requests Exist

Pull Requests prevent accidental damage.

Without Pull Requests:

Developer edits main directly
Mistake breaks entire project

With Pull Requests:

Developer creates branch
Makes changes safely
Requests review
Merge only if approved

Main remains safe.

---

# Real World Example

Imagine a company website.

Main branch:

```
Live website
```

Developer creates branch:

```
add-login-feature
```

Developer builds login system.

Before adding to main, developer creates Pull Request.

Team reviews code.

If approved → merge
If rejected → fix issues

This protects production code.

---

# Step 1 — Create a Branch Locally

Open terminal.

Run:

```bash
git checkout -b add-feature
```

Make changes.

Example:

Edit notes.txt

Add:

```
This feature was added using pull request workflow.
```

Save file.

Commit changes:

```bash
git add .
git commit -m "Added new feature"
```

Push branch to GitHub:

```bash
git push origin add-feature
```

Branch is now on GitHub.

---

# Step 2 — Open GitHub Repository

Go to:

```
https://github.com/yourusername/my-first-project
```

GitHub will show:

```
Compare & pull request
```

Click it.

---

# Step 3 — Create Pull Request

GitHub shows:

```
Base branch: main
Compare branch: add-feature
```

This means:

Merge add-feature into main.

Enter title:

```
Added new feature
```

Enter description:

```
This pull request adds new feature safely.
```

Click:

```
Create pull request
```

Pull Request is now created.

---

# Step 4 — Review Pull Request

GitHub shows:

* Files changed
* Lines added
* Lines removed

You can review all changes.

This ensures safety.

---

# Step 5 — Merge Pull Request

Click:

```
Merge pull request
```

Confirm merge.

GitHub merges branch into main.

Main is now updated safely.

---

# Step 6 — Delete Branch (Optional)

After merge, branch is no longer needed.

GitHub shows:

```
Delete branch
```

Click it.

Cleanup keeps repository organized.

---

# What Happens Internally

Before merge:

```
main:        A --- B --- C

add-feature:           D --- E
```

After merge:

```
main: A --- B --- C --- D --- E
```

History is preserved.

Nothing is lost.

---

# Why Companies Require Pull Requests

Pull Requests allow:

* Code review
* Bug detection
* Safe merging
* Team collaboration
* Change tracking

This prevents production failures.

Every professional team uses Pull Requests.

---

# Pull Request Workflow Summary

Step 1 — Create branch
Step 2 — Make changes
Step 3 — Commit changes
Step 4 — Push branch
Step 5 — Create Pull Request
Step 6 — Review changes
Step 7 — Merge safely

This is professional workflow.

---

# Summary

You can now:

* Create branches
* Push branches to GitHub
* Create Pull Requests
* Review changes
* Merge safely

You now understand professional GitHub workflow.

---

# Result

You have completed Part 2 — Professional Workflow.

You can now work safely in teams.

You are using GitHub like a professional developer.
