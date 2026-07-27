# 🌱 Git Basics

A beginner-friendly guide to the core Git commands you'll use every day in **Practice_Pravidham**.

---

## 1. `git clone`
Downloads a copy of the repository to your computer.

```bash
git clone https://github.com/<username>/Practice_Pravidham.git
```
> Use this only **once**, when you first set up the repo on a new machine.

---

## 2. `git status`
Shows what has changed in your working folder — new files, edited files, staged files.

```bash
git status
```
> Run this often. It tells you exactly what Git is about to do next.

---

## 3. `git add`
Stages your changes so Git knows you want to include them in the next commit.

```bash
git add filename.cpp      # stage a single file
git add .                 # stage everything in the current folder
```

---

## 4. `git commit`
Saves your staged changes as a snapshot, with a message describing what you did.

```bash
git commit -m "Added Two Sum solution in LeetCode folder"
```
> Write clear, meaningful messages — not just "update" or "fix".

---

## 5. `git push`
Uploads your local commits to GitHub so everyone can see them.

```bash
git push origin main
```

---

## 6. `git pull`
Downloads the latest changes from GitHub and merges them into your local copy.

```bash
git pull origin main
```
> **Always pull before you start working** to avoid conflicts.

---

## 7. `git log`
Shows the history of commits — who did what, and when.

```bash
git log
git log --oneline    # compact one-line view
```

---

## 8. `git branch`
Lists, creates, or switches between branches.

```bash
git branch                 # list branches
git branch new-feature      # create a branch
git checkout new-feature    # switch to it
```
> Since each member works in their own folder on `main`, branches are optional here — but useful if you want to experiment safely before merging.

---

## ✅ Quick Reference Table

| Command | Purpose |
|---|---|
| `git clone` | Copy a repo to your machine |
| `git status` | Check current changes |
| `git add` | Stage changes |
| `git commit` | Save a snapshot with a message |
| `git push` | Upload commits to GitHub |
| `git pull` | Download latest changes |
| `git log` | View commit history |
| `git branch` | Manage branches |

---

💡 **Tip:** The golden order of daily commands is:
```
git pull origin main
... do your work ...
git add .
git commit -m "message"
git push origin main
```
