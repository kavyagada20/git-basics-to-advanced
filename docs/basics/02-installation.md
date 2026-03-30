# ⚙️ Installing Git

---

## 📌 Overview

Before using Git, you need to install it on your system and configure it with your identity.

This guide covers installation for:
- Windows
- macOS
- Linux

---

## 🖥️ Install Git on Different OS

### 🪟 Windows

1. Go to the official Git website: https://git-scm.com/
2. Download the installer
3. Run the setup and keep default settings (recommended)
4. Install Git Bash along with Git

✅ After installation, open **Git Bash**

---

### 🍎 macOS

#### Method 1: Using Homebrew
```bash
brew install git
Method 2: Using Xcode Command Line Tools
xcode-select --install

🐧 Linux
Ubuntu / Debian
sudo apt update
sudo apt install git
Fedora
sudo dnf install git
Arch Linux
sudo pacman -S git
✅ Verify Installation

Check if Git is installed correctly:

git --version

👉 Example output:

git version 2.x.x
👤 Initial Configuration

Set your username and email (important for commits):

git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
🔍 Check Configuration
git config --list
⚙️ Optional Configurations
Set Default Editor (VS Code)
git config --global core.editor "code --wait"
Enable Colored Output
git config --global color.ui auto
📁 Default Branch Name (Optional)

Set default branch to main:

git config --global init.defaultBranch main
🧠 Best Practices
Always configure your username and email
Use a consistent email (same as GitHub)
Keep Git updated
🎯 Summary
Git can be installed on all major OS
Configuration is required before use
Verification ensures proper setup
➡️ Next Step

Continue to:

👉 03-git-init-clone.md