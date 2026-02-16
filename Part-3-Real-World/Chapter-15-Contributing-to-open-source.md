# Chapter 15 — Contributing to Open Source Projects

Open source is the foundation of modern software.

Most software you use today is built using open source.

Examples include:

* Linux
* Python
* Git
* VSCode

Open source means the code is publicly available.

Anyone can view it, use it, and improve it.

This allows developers around the world to collaborate.

---

# Why Open Source Matters

Open source helps you:

* Learn from real projects
* Improve your skills
* Build credibility
* Collaborate with global developers
* Strengthen your GitHub profile

Many developers get hired because of open source contributions.

It proves you can work in real projects.

---

# What is a Contribution?

A contribution means improving a project.

Examples:

* Fixing a bug
* Improving documentation
* Adding a feature
* Fixing spelling mistakes
* Adding examples

Even small contributions matter.

Your first contribution can be very simple.

---

# How Open Source Projects Are Structured

Open source repositories look like normal repositories.

Example:

```
project-name/
│
├── README.md
├── src/
├── docs/
└── requirements.txt
```

But they also include contribution guidelines.

Example:

```
CONTRIBUTING.md
```

This file explains how to contribute.

---

# Step 1 — Find an Open Source Project

Go to:

https://github.com

Search for:

* python projects
* beginner projects
* documentation projects

Look for repositories with:

* Active commits
* Clear README
* Contribution guidelines

Good projects welcome beginners.

---

# Step 2 — Fork the Repository

Fork means copying the repository to your GitHub account.

Click:

Fork button (top right)

GitHub creates your copy.

Now you own your version.

This allows you to make changes safely.

---

# Step 3 — Clone Your Fork

Clone your fork to your computer.

Run:

```bash
git clone https://github.com/yourusername/project-name.git
```

Enter project folder:

```bash
cd project-name
```

You now have the project locally.

---

# Step 4 — Create a New Branch

Never modify main branch.

Create a branch:

```bash
git checkout -b fix-typo
```

Now you work safely.

---

# Step 5 — Make Your Changes

Edit files.

Example:

Fix spelling mistake in README.md

Save the file.

---

# Step 6 — Commit Your Changes

Run:

```bash
git add .
git commit -m "Fixed spelling mistake in README"
```

This saves your change.

---

# Step 7 — Push to Your Fork

Run:

```bash
git push origin fix-typo
```

This uploads your branch to your GitHub fork.

---

# Step 8 — Create Pull Request

Go to your GitHub fork.

Click:

Compare & Pull Request

GitHub will show your changes.

Click:

Create Pull Request

This sends your changes to original project.

---

# What Happens Next

Project maintainers review your changes.

They may:

* Accept your contribution
* Suggest improvements
* Ask questions

If accepted, your contribution becomes part of project.

This is a major milestone.

You have contributed to open source.

---

# What You Gain

You gain:

* Real project experience
* Public proof of skill
* GitHub contribution history
* Credibility as developer

This builds your professional identity.

---

# Important Rule

Always create branch.

Never push directly to main.

Branch → Commit → Push → Pull Request

This is the professional workflow.

---

# Summary

You learned:

* What open source is
* Why open source matters
* How to fork a repository
* How to make changes safely
* How to create a pull request

You can now contribute to global software projects.

You are no longer just a learner.

You are a contributor.
