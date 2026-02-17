# Chapter 1 — What is Git, and Why It Exists

## The Fundamental Problem: Software Changes Constantly

Software isn’t written once — it evolves:

- Features are added  
- Bugs get fixed  
- Performance gets improved  
- New ideas are tested

Every change modifies files. Without a system to track these changes:

- Files get overwritten  
- Previous work gets lost  
- It’s hard to understand what changed or why

That’s where **version control** comes in: a system that records and manages changes to your project over time. :contentReference[oaicite:2]{index=2}

---

## What Git Actually Is

**Git** is a **distributed version control system** that:

- Records snapshots of your project over time  
- Tracks what changed, when it changed, and who changed it  
- Lets you **go back to any previous version instantly**  
- Prevents lost work and confusion

If you think of your project like a story, Git is like a **time machine for your files** — you can revisit any point in the story whenever you want. :contentReference[oaicite:3]{index=3}

---

## A Simple Example

### 🤷 Life Without Git

Imagine you’re building a Notes App. You might end up with folders like:

```
    notes_app
    notes_app_new
    notes_app_final
    notes_app_final_v2
    notes_app_final_USE_THIS
```

It’s easy to get confused — which one is the real final version?

---

### 👍 Life With Git

With Git:

- You have one project folder  
- Git tracks every version internally  
- You can review and undo changes  
- You never lose work by mistake

---

## Why Git Was Created

Git was created in **2005 by Linus Torvalds** (the creator of Linux) because:

- He needed a system that could handle a large, fast‑moving codebase  
- He wanted tools that would **never lose history**  
- The system had to support **thousands of contributors efficiently** :contentReference[oaicite:4]{index=4}

Today, Git is the foundation of modern software development.

---

## Git vs GitHub: Know the Difference

| **Git** | **GitHub** |
|---------|------------|
| Runs locally on your computer | Runs on the internet |
| Tracks changes | Stores projects online |
| Version control tool | Hosting platform |
| Works offline | Requires internet |

> **Git** = the engine that tracks history  
> **GitHub** = the platform that hosts and shares those histories online :contentReference[oaicite:5]{index=5}

---

## Why Every Developer Uses Git

Git gives you:

- **Safety** — history is never lost  
- **Control** — understand what changed and why  
- **Confidence** — experiment and undo safely  
- **Collaboration** — work with others without overwriting each other’s work

Without Git, development is fragile. With Git, development becomes structured, reliable, and professional.

---

## Summary

Git is a tool that tracks changes in your files and lets you manage software projects reliably. It is the foundation of modern software engineering. :contentReference[oaicite:6]{index=6}

---

Next up, in **Chapter 2**, we’ll learn *how Git tracks changes internally*.
