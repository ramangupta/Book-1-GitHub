# Chapter 2 — Installing Git and Creating Your First Repository

In this chapter, you will install Git and create your first repository.

This is where theory becomes real.

---


## Step 1 — Check if Git is Already Installed

Open Terminal and run:

```bash
git --version
```

If Git is installed, you will see something like:

```bash
git version 2.34.1
```

If not installed, install using:

### Windows
1. Go to https://git‑scm.com/download/win  
2. Download the installer and run it.  
3. Use the **default options** unless you have a reason to change them.

### macOS
1. On macOS, you can install Git using Homebrew:
   ```bash
   brew install git

### Linux

```bash
sudo apt update
sudo apt install git
```

(Make sure the installation completes without errors.)

Verify again:

```bash
git --version
```

## Step 2 — Configure Git (First Time Only)

Git needs to know your identity so it can label your commits correctly.

Open your terminal and run the following commands:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```
Example:

```text
git config --global user.name "Ian Cooper"
git config --global user.email "ic@example.com"
```

Verify configuration:

```bash
git config --list
```

## Step 3 — Create Your First Project Folder

Create a folder:

```bash
mkdir my-first-project
cd my-first-project
```

Create a file:

```bash
touch notes.txt
```

Open in VSCode:

```bash
code .
```

Write inside notes.txt:

```text
This is my first Git project.
```

Save the file. 

## Step 4 — Initialize Git Repository

Run:

```bash
git init
```

Output:

```bash
Initialized empty Git repository
```

Git is now tracking this folder.

This folder is now called a repository.

### What is a Repository?

A repository (repo) is a project tracked by Git.

It contains:

- Your files
- Git tracking information
- Change history

Git creates a hidden folder:

```bash
.git/
```

This stores all version history.

## Step 5 — Check Git Status

Run:

```bash
git status
```

Output:

```bash
Untracked files:
  notes.txt
```

Git sees the file, but is not tracking it yet.

## Step 6 — Add File to Git

Run:

```bash
git add notes.txt
```

This tells Git:

Track this file.

Check status again:

```bash
git status
```

You will see:

```bash
Changes to be committed:
  notes.txt
```

## Step 7 — Save First Version (Commit)

Run:

```bash
git commit -m "Initial commit"
```

Output:

```bash
1 file changed
```

Git has now saved the first version of your project.

This is called a commit.

### What is a Commit?

A commit is a snapshot of your project at a specific time.

It includes:

- File changes
- Timestamp
- Author
- Message

Each commit is permanent.

## Step 8 — View Commit History

Run:

```bash
git log
```

You will see:

```bash
commit 7f3a8c2...
Author: Your Name
Message: Initial commit
```

This is your project history.

### Summary

You have now:

- Installed Git
- Configured Git
- Created a repository
- Added a file
- Made your first commit
- Viewed commit history

You are now using Git.