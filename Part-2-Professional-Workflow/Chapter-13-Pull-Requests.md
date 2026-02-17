# Chapter 13 — Pull Requests (Professional Team Collaboration)

Until now, you learned how to:

* Create branches
* Make changes
* Commit work
* Merge branches

You have been working alone.

But professional software is built by teams.

Multiple developers work on the same project.

Pull Requests make this collaboration safe and organized.

---

## What is a Pull Request

A Pull Request is a request to merge your branch into another branch.

Usually, this means merging your branch into the main branch.

It is called a Pull Request because you are requesting the project to pull your changes into the main code.

Pull Requests allow changes to be reviewed before merging.

This protects the project from errors.

---

## Why Pull Requests are Important

Professional teams do not merge branches directly.

Instead, they create Pull Requests.

This allows teams to:

* Review code
* Detect mistakes
* Discuss changes
* Ensure quality

Pull Requests act as a safety checkpoint.

They ensure only safe and correct code enters the main branch.

---

## Real-World Workflow

Professional workflow follows these steps:

Step 1 — Create branch

```bash
git checkout -b new-feature
```

Step 2 — Make changes

```bash
nano feature.txt
```

Step 3 — Commit changes

```bash
git add .
git commit -m "Added new feature"
```

Step 4 — Push branch to GitHub

```bash
git push origin new-feature
```

Your branch is now available on GitHub.

---

## Creating Pull Request on GitHub

Go to your repository on GitHub.

You will see a message:

```
Compare & pull request
```

Click this button.

GitHub will show:

Base branch: main
Compare branch: new-feature

Click:

```
Create Pull Request
```

Your Pull Request is now created.

---

## What Happens in a Pull Request

GitHub shows:

* Files changed
* Lines added
* Lines removed

This allows review of changes.

Team members can:

* Review code
* Suggest changes
* Approve changes

This ensures safety and quality.

---

## Merging Pull Request

After review, click:

```
Merge Pull Request
```

GitHub will merge the branch into main.

Your feature becomes part of the main project.

The project is safely updated.

---

## Pull Request vs Direct Merge

Direct merge:

Fast
But risky

Pull Request merge:

Safe
Reviewed
Professional

Professional teams always use Pull Requests.

---

## After Merge

Your branch is no longer needed.

GitHub may show:

```
Delete branch
```

Click it to clean up.

Your changes remain safely in main.

The branch is removed.

---

## Professional Team Example

Developer A:

Creates branch
Adds feature
Creates Pull Request

Team reviews code

Pull Request is approved

Changes merged into main

Project is safely updated.

This workflow is used by companies worldwide.

---

## Git and GitHub Roles

Git handles:

* Local changes
* Commits
* Branches

GitHub handles:

* Pull Requests
* Code review
* Team collaboration

Together, they create a complete professional system.

---

## Commands Learned

Push branch:

```bash
git push origin branch-name
```

Create Pull Request:

Done on GitHub website

Merge Pull Request:

Done on GitHub website

---

## What You Achieved

You learned the most important professional Git workflow.

You can now:

* Create feature branches
* Push branches to GitHub
* Create Pull Requests
* Merge changes safely
* Collaborate professionally

This is how real software is built.

You now understand professional Git and GitHub workflow.
