🛠️ VS Code Setup for C++ & Git

A quick setup guide so every team member has a consistent development environment.

1. Install VS Code

Download from: https://code.visualstudio.com

2. Install a C++ Compiler
Windows:Use Through MSYS-2
then install g++


bash
  xcode-select --install
  
Linux: Usually pre-installed; otherwise:
bash
  sudo apt install g++

Verify installation:

bash
g++ --version

3. Recommended VS Code Extensions
Extension	Purpose
C/C++ (Microsoft)	IntelliSense, debugging, code navigation
Code Runner	Run code with a single click
GitLens	Enhanced Git history & blame view
Git Graph	Visualize branches and commits
Markdown All in One	Easier README/Markdown editing
4. Configure Code Runner (Optional but Handy)



5. Git Setup Inside VS Code
Install Git from https://git-scm.com/downloads
Open VS Code → Terminal → run:
bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
Clone the repo directly from VS Code: Ctrl+Shift+P → Git: Clone → paste the repo URL.

7. Recommended Folder Workflow in VS Code
Open your own member folder as the working directory to avoid clutter:
bash
  code Practice_Pravidham/Chandan

  
✅ Quick Setup Checklist
 VS Code installed
 g++ compiler installed & verified
 C/C++ and GitLens extensions installed
 Git configured with name & email
 Repository cloned locally
