# 🛠️ VS Code Setup for C++ & Git

A quick setup guide so every team member has a consistent development environment.

---

## 1. Install VS Code
Download from: https://code.visualstudio.com

---

## 2. Install a C++ Compiler

- **Windows:** Install [MinGW-w64](https://www.mingw-w64.org) or use WSL with `g++` pre-installed.
- **macOS:** Install Xcode Command Line Tools:
  ```bash
  xcode-select --install
  ```
- **Linux:** Usually pre-installed; otherwise:
  ```bash
  sudo apt install g++
  ```

Verify installation:
```bash
g++ --version
```

---

## 3. Recommended VS Code Extensions

| Extension | Purpose |
|---|---|
| C/C++ (Microsoft) | IntelliSense, debugging, code navigation |
| Code Runner | Run code with a single click |
| GitLens | Enhanced Git history & blame view |
| Git Graph | Visualize branches and commits |
| Markdown All in One | Easier README/Markdown editing |

---

## 4. Configure Code Runner (Optional but Handy)

In VS Code settings (`settings.json`), add:
```json
{
  "code-runner.executorMap": {
    "cpp": "cd $dir && g++ -std=c++17 $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt"
  },
  "code-runner.runInTerminal": true
}
```
This compiles with C++17 and runs your file with `Ctrl+Alt+N`.

---

## 5. Git Setup Inside VS Code

1. Install Git from https://git-scm.com/downloads
2. Open VS Code → Terminal → run:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   ```
3. Clone the repo directly from VS Code:
   `Ctrl+Shift+P` → **Git: Clone** → paste the repo URL.

---

## 6. Recommended Folder Workflow in VS Code

- Open your **own member folder** as the working directory to avoid clutter:
  ```bash
  code Practice_Pravidham/Chandan
  ```
- Use the built-in **Source Control panel** (`Ctrl+Shift+G`) to stage, commit, and push without typing every command manually.

---

## ✅ Quick Setup Checklist

- [ ] VS Code installed
- [ ] g++ compiler installed & verified
- [ ] C/C++ and GitLens extensions installed
- [ ] Git configured with name & email
- [ ] Repository cloned locally
