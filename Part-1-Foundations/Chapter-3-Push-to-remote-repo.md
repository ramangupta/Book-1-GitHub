# Chapter 3 — Connecting Your Project to GitHub

Until now, your repository exists only on your local computer.

This means:

- If your computer crashes, your project is lost
- No one else can see your work
- You cannot collaborate
- Your project is not backed up

GitHub solves this.

GitHub stores your repository on the internet.

This allows you to:

- Back up your project safely
- Access it from anywhere
- Share it with the world
- Build a public portfolio

---

## Step 1 — Create a GitHub Account

Go to:

https://github.com

Click:

Create Account

Follow the instructions.

Choose a professional username.

---

## Step 2 — Create a New Repository on GitHub

After login, click the "+" icon at top right.

Click:

New repository

You will see a form.

Fill it like this:

Repository name:

my-first-project

Description:

My first GitHub project

Select:

Public

DO NOT check:

Initialize with README

Click:

Create repository


---

## Step 3 — GitHub Will Show Connection Commands

GitHub will show something like:

```bash
git remote add origin https://github.com/yourusername/my-first-project.git
git branch -M main
git push -u origin main
```

These commands connect your local repository to GitHub.

## Step 4 - Run these commands in your terminal

Make sure you are inside your project folder:

```bash
cd my-first-project
```

Now run:

```bash
git remote add origin https://github.com/yourusername/my-first-project.git
```

This connects your local repository to GitHub.

Now run:

```bash
git branch -M main
```

This sets the main branch. 

Now run:

```bash
git push -u origin main
```

This uploads your project to GitHub.

## Step 5 - Authentication

GitHub may ask for:

Username:
Password or Personal Access Token

Enter your GitHub credentials.

## Step 6 — Verify Upload

Go to your GitHub page:

https://github.com/yourusername/my-first-project

You will see:

```bash
notes.txt
```

Your project is now online !

## What Just Happened?

Your project now exists in two places:

**Local repository**  
Stored on your computer

**Remote repository**  
Stored on GitHub


Git keeps them synchronized.

## Important Concept — Remote Repository

Remote repository = version stored on GitHub.

Local repository = version stored on your computer.

You push changes from local → remote.

You pull changes from remote → local.

---

## Summary

You have now:

* Created a GitHub account
* Created a GitHub repository
* Connected your local project to GitHub
* Uploaded your project online

You now have a public software project.

You are officially using GitHub.







