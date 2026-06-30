# 100hires-setup

Setup notes and documentation for onboarding with **Cursor**, **GitHub**, **Claude Code**, and **Git**.

This repository records the tools installed, the steps taken during setup, and how common issues were resolved.

---

## Tools & accounts

### Installed


| Tool                            | Purpose                        |
| ------------------------------- | ------------------------------ |
| **Cursor**                      | AI-powered code editor         |
| **Git**                         | Version control                |
| **Claude extension for Cursor** | AI assistant inside the editor |
| **GitHub**                      | Remote repository hosting      |


### Accounts created

- **Cursor** — signed in with a Google account
- **GitHub** — new account created and connected to Cursor

---

## Setup walkthrough

### 1. Install Cursor

1. Reviewed the onboarding email (with help from ChatGPT).
2. Downloaded Cursor from the official site.
3. Handled the Windows **"Windows protected your PC"** dialog by selecting **Run anyway**.
4. Accepted the license agreement and completed the installer (destination, Start Menu folder, additional tasks).
5. Signed in to Cursor using a Google account.

### 2. Connect GitHub

1. Created a GitHub account.
2. Connected GitHub to Cursor and authorized access.
3. Retried the connection after a session-expired error (see [Troubleshooting](#troubleshooting)).

### 3. Install the Claude extension

1. Opened the extension panel in Cursor (see [Troubleshooting](#troubleshooting) if you cannot find it).
2. Installed the Claude extension.

### 4. Open a repository in Cursor

1. Created a GitHub repository.
2. Watched a YouTube tutorial on opening a GitHub repo in Cursor and followed the steps shown.
3. Opened the repository in Cursor and learned how to edit code.

### 5. Commit, push, and document

1. Enabled commit and push in Cursor.
2. Configured Git username and email when prompted (see [Troubleshooting](#troubleshooting)).
3. Documented the full setup process in this repository.

---

## Troubleshooting

Each issue below includes what happened and how it was fixed.

### Session expired while connecting GitHub

**What happened:** The GitHub connection session expired before authorization finished.

**Fix:** Retried the connection through GitHub and completed the process.

### Could not find the extension panel

**What happened:** The extension panel was not obvious in the Cursor UI at first.

**Fix:** Used ChatGPT to locate the extension panel, then installed the Claude extension.

### Opening the repository in Cursor

**What happened:** It was unclear how to open a GitHub repository inside Cursor.

**Fix:** Watched a YouTube tutorial and followed the demonstrated steps.

### Git username and email not configured

**What happened:** While trying to commit and push, a dialog appeared:

> Make sure you configure your username and usermail in Git.

**Fix:** Looked up the solution via Google AI Search, then configured the username and user email in Git Bash:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

## Quick reference


| Task                   | Where to do it                      |
| ---------------------- | ----------------------------------- |
| Edit code              | Cursor editor                       |
| Install extensions     | Cursor extension panel              |
| Create / manage repos  | GitHub                              |
| Commit and push        | Cursor (Source Control) or Git Bash |
| Configure Git identity | Git Bash (`git config --global …`)  |


