# 🔄 GitHub Workflow — Practice_Pravidham

This document explains the **daily workflow** every team member follows.

---

## 🗺️ Overview

Each member (Chandan, Pavan, Kanhaiya, Shreya, Aishwarya) works **only inside their own folder**. There is no merging of solutions between members — this repo is a shared archive, not a shared codebase.

---

## 📅 Daily Workflow Steps

### Step 1 — Pull the latest changes
Before touching anything, sync your local copy with GitHub:
```bash
git pull origin main
```
This prevents conflicts caused by outdated local files.

### Step 2 — Solve your problem(s)
Work inside your own folder, e.g.:
```
Chandan/LeetCode/two-sum.cpp
Chandan/Codeforces/1523A.cpp
```

### Step 3 — Check what changed
```bash
git status
```

### Step 4 — Stage your changes
```bash
git add .
```

### Step 5 — Commit with a meaningful message
```bash
git commit -m "Chandan: Solved Two Sum (LeetCode) using HashMap"
```

### Step 6 — Push to GitHub
```bash
git push origin main
```

---

## 🔁 Visual Flow

```
 ┌────────────┐     ┌──────────────┐     ┌───────────┐     ┌────────────┐
 │ git pull   │ --> │ Solve problem│ --> │ git add . │ --> │ git commit │
 └────────────┘     └──────────────┘     └───────────┘     └─────┬──────┘
                                                                  │
                                                          ┌───────▼───────┐
                                                          │  git push     │
                                                          └───────────────┘
```

---

## ⚠️ Handling Conflicts

Since everyone works in **separate folders**, conflicts should be rare. If one ever occurs:

1. Don't panic.
2. Run `git status` to see the conflicting file.
3. Open the file — Git marks conflicts with `<<<<<<<`, `=======`, `>>>>>>>`.
4. Keep the correct version, remove the markers.
5. `git add .` → `git commit` → `git push`.
6. If unsure, ask a teammate before pushing.

---

## 📌 Weekly Checklist

| Task | Frequency |
|---|---|
| Pull latest changes | Every session |
| Solve & commit problems | Daily |
| Review own folder structure | Weekly |
| Update README/profile progress | Monthly |

---

## ✅ Golden Rule

> **Pull → Work → Add → Commit → Push**
> Every single day, without skipping steps.
