# Version Control Made Simple: Git, GitHub & VS Code

**Duration:** ~1 Hour 50 Minutes (110 minutes)

**Format:** 30% Concepts / 70% Hands-on Practice

**Goal:** Help non-technical learners confidently save, track, and share their work using Git, GitHub, and VS Code.

Watch before class: [Git & GitHub Zero to Hero](https://youtu.be/1I79WAZ4uSU) *(15 mins)*

---

## 🎯 Learning Objectives

By the end of this session, you will be able to:

1. Explain what Git and GitHub are — and why they matter
2. Describe the difference between "local" (your computer) and "remote" (GitHub)
3. Use the essential Git actions: Stage → Commit → Push → Pull
4. Connect VS Code to GitHub and keep your work in sync
5. *(Optional)* Explain what Google Colab is and how it connects to GitHub

---

## 🕒 Session Agenda

| Time | Activity | Type |
|------|----------|------|
| **0:00 – 0:15** | Module 1: What is Git & GitHub? | Concepts (15 min) |
| **0:15 – 0:30** | Module 2: Local vs. Remote | Concepts + Demo (15 min) |
| **0:30 – 0:33** | Setup Check (verify everyone's tools work) | Checkpoint (3 min) |
| **0:33 – 0:55** | Exercise A: Your First Repository & Commit | Hands-on (22 min) |
| **0:55 – 1:25** | Exercise B: Make Changes, Stay in Sync & Resolve a Conflict | Hands-on (30 min) |
| **1:25 – 1:40** | Exercise C: Pair Collaboration | Hands-on (15 min) |
| **1:40 – 1:50** | Module 3: What is Colab? + Self-Check + Wrap Up | Concepts (10 min) |

---

## 📘 Module 1: What is Git & GitHub? (15 mins)

> **Instructor note:** open with a 2-minute recap of the pre-class video ([Git & GitHub Zero to Hero](https://youtu.be/1I79WAZ4uSU)) and a quick "what stuck / what confused you?" — don't assume everyone watched it.

### The Problem Git Solves

Imagine you are writing an important report. You save it as `Report_Final.docx`. Then you make more changes: `Report_Final_v2.docx`. Then `Report_Final_REAL_v3.docx`. Sound familiar?

This is confusing, takes up space, and makes it hard to know which version is the "real" one.

**Git** solves this by acting like a **time machine** for your files. Every time you tell it to, Git takes a *snapshot* of your work. You can label each snapshot with a description, and jump back to any snapshot at any time — without creating dozens of copies.

### Git vs. GitHub — What's the Difference?

Think of it this way:

> **Git** is the camera that takes the snapshots.  
> **GitHub** is the photo album in the cloud where you store and share them.

| | Git | GitHub |
|---|---|---|
| What is it? | Software installed on your computer | A website (github.com) |
| What does it do? | Tracks changes to your files | Stores and shares those changes online |
| Do you need the internet? | No | Yes |

You use Git *locally* (on your computer), and GitHub *remotely* (in the cloud).

### Why Does This Matter?

- **Backup:** Your work is safely stored on GitHub, even if your laptop breaks.
- **History:** You can always go back to an earlier version.
- **Sharing:** Anyone with the link can view (or contribute to) your work.
- **Collaboration:** Multiple people can work on the same project without overwriting each other.

### Key Terms to Know

| Term | Plain English |
|------|--------------|
| **Repository (Repo)** | A project folder that Git is tracking |
| **Commit** | A saved snapshot with a label describing what changed |
| **Push** | Sending your snapshots from your computer up to GitHub |
| **Pull** | Downloading the latest snapshots from GitHub to your computer |
| **Clone** | Making your own full copy of a GitHub project onto your computer, like downloading a shared Google Doc to edit offline |
| **Branch** | A safe side-copy of your project to try changes without touching the main version, like "Save As" a draft before editing the original |

---

## 📘 Module 2: Local vs. Remote (15 mins)

### Two Places Your Work Lives

When you use Git and GitHub, your project exists in two places:

```
Your Computer (Local)          GitHub (Remote)
┌─────────────────────┐       ┌─────────────────────┐
│  Working Files      │       │                     │
│  (what you edit)    │ ─────►│  GitHub Repository  │
│                     │ Push  │  (the cloud copy)   │
│  Commit History     │◄───── │                     │
│  (your snapshots)   │ Pull  └─────────────────────┘
└─────────────────────┘
```

- **Local** = the files on your laptop in VS Code. This is where you do your work.
- **Remote** = the copy stored on GitHub. This is the shared, backed-up version.

### The Three-Zone Mental Model (Inside VS Code)

Your change passes through **three zones** on your computer — Working Files → Staging → Commit — and then a fourth action, **Push**, sends it to GitHub:

```
[1] Working Files  →  [2] Staging Area  →  [3] Local Commit  →  GitHub
 (you edited it)      (you selected it)     (you saved it)      (you shared it)
```

1. **Working Files** — You make changes (type, edit, delete).
2. **Staging Area** — You choose *which* changes to include in the next snapshot (clicking the `+` in VS Code).
3. **Commit** — You take the snapshot and write a label describing what you did.
4. **Push** — You send the snapshot up to GitHub.

> **Analogy:** Think of it like packing a suitcase. You lay out clothes (Working Files), choose what to pack (Staging), zip up the suitcase (Commit), then check it in at the airport (Push).

> ⚠️ **About the "Sync Changes" button:** VS Code bundles **Pull then Push into one click** called *Sync Changes*. Handy, but remember they're still two separate directions — **Push** sends your work up, **Pull** brings others' work down. The cheatsheet shows them as separate `git push` / `git pull` so you keep the two directions clear in your head.

### Demo: Cloning a Repository

*The instructor will demonstrate cloning this repo to show how a remote repository becomes a local one.*

1. Go to a GitHub repository page
2. Click the green **Code** button → copy the HTTPS URL
3. Open VS Code → `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) → type **Git: Clone**
4. Paste the URL → choose a folder on your computer → click **Open**

Now the project is on your computer. You can edit it locally, then push changes back to GitHub.

---

## ✅ Setup Check (3 mins — do this before Exercise A)

*Don't skip this. It catches broken setups now, instead of 40 minutes into the exercise. If any item is ❌, flag an instructor/TA before continuing — the rest of the class depends on these working.*

- [ ] **Git installed** — VS Code terminal (`` Ctrl+` `` / `` Cmd+` ``), type `git --version`, see `git version 2.x.x`
- [ ] **Name/email set** — type `git config --global --list`, see your `user.name` and `user.email`
- [ ] **Signed into GitHub in VS Code** — click the account icon (bottom-left circle); it should show your GitHub username
- [ ] **You can log in to github.com** in a browser

> 🛟 **If your setup can't be fixed in a few minutes:** don't sit out — do the whole session on **github.com in the browser** instead. You can create repos, add/edit files, and commit entirely on the website (pencil icon → edit → Commit changes). You'll miss the VS Code steps but keep every Git concept. Fix your local setup after class using `pre-class.md` + the troubleshooting guide.

> **Instructor note:** GitHub redesigns its UI often. Before class, click through the exercise once and confirm button names/locations below still match ("+ icon", "green Code button", "pencil icon", "Settings → Collaborators").
>
> **Instructor note — network failure plan:** this session is 100% dependent on Wi-Fi and GitHub being up, and classroom Wi-Fi with 30 people cloning at once *will* struggle. If the network dies: switch to concepts + the merge-conflict demo (steps 2–5 work fully offline in a local repo), and run the push/pull portions when it recovers.

---

## 💻 Exercise A: Your First Repository & Commit (22 mins)

*Goal: Create a GitHub repository and make your first commit using VS Code.*

### Step 1 — Create a Repository on GitHub

1. Go to [github.com](https://github.com) and log in.
2. Click the **+** icon (top right) → **New repository**.
3. Fill in:
   - **Repository name:** `my-learning-journal`
   - **Description:** `My notes from the Git & GitHub session`
   - **Visibility:** Public
   - **Check the box:** ✅ Add a README file
4. Click **Create repository**.

> ⚠️ **"Public" means anyone on the internet can read this repo.** That's fine for practice notes — but never put passwords, personal data, or private work in a public repo.

✅ You now have a repository on GitHub! Notice the `README.md` file that was created automatically.

### Step 2 — Clone It to Your Computer

1. On your new GitHub repository page, click the green **Code** button.
2. Make sure **HTTPS** is selected. Copy the URL — it looks like `https://github.com/yourname/my-learning-journal.git`, but with **your actual GitHub username** in place of `yourname` (don't type "yourname" literally).
3. Open **VS Code**.
   - *Windows users:* if you set up WSL in pre-class, click **Connect to WSL** on the blue remote-window button (bottom-left) first. ⚠️ Once connected, your files live **inside WSL (a Linux workspace), not in normal Windows folders** — so reopen them through VS Code, not Windows File Explorer.
4. Press `Ctrl+Shift+P` (Windows) or `Cmd+Shift+P` (Mac) to open the Command Palette.
5. Type **Git: Clone** and select it.
6. Paste the URL you copied.
7. Choose **one folder you'll remember** — e.g. make a `GitHub` folder directly in your home folder (`C:\Users\you\GitHub` on Windows, `/Users/you/GitHub` on Mac) and always clone there. Write down where you put it.
   - ⚠️ **Avoid Documents and Desktop** — on many machines those are synced by OneDrive (Windows) or iCloud (Mac), and cloud sync fighting over Git's hidden files causes locked files and corrupted repos that are very hard to diagnose.
8. When prompted, click **Open Repository**.
9. If VS Code asks **"Do you trust the authors of the files in this folder?"** — click **Yes, I trust the authors**. (Clicking "No" silently disables Git features and it's hard to notice why. If you clicked No by accident: `Ctrl+Shift+P` → **Workspaces: Manage Workspace Trust** → Trust.)

✅ Your repository is now on your computer and open in VS Code!

> 💡 **Next time you want this project back:** don't re-clone it. Open VS Code → **File → Open Recent** (or **Open Folder** → the folder from step 7). Re-cloning makes confusing duplicates.

### Step 3 — Create Your First File

1. In VS Code's left sidebar (Explorer), right-click in the empty space → **New File**.
2. Name the file `notes.txt`.
3. Type something inside — for example:
   ```
   Day 1: Git is like a time machine for files.
   GitHub is where those snapshots live in the cloud.
   ```
4. Save the file: `Ctrl+S` (Windows) or `Cmd+S` (Mac).

### Step 4 — Stage, Commit & Push

1. Click the **Source Control** icon in the left sidebar (it looks like a branching diagram, or press `Ctrl+Shift+G`).
2. You'll see `notes.txt` listed under **Changes**.
3. **Stage:** Hover over `notes.txt` and click the **+** button. It moves to **Staged Changes**.
4. **Commit:** Type a message in the box at the top, for example: `Add my first notes`. Then click the **✔ Commit** button (or press `Ctrl+Enter`).
5. **Push:** Click the **Sync Changes** button (or the cloud icon at the bottom of the screen).
6. **Authorize GitHub (first push only):** A browser window will likely pop up asking you to authorise GitHub. This is expected — it's the #1 spot beginners get stuck.
   - Click the green **Authorize** button.
   - **Then return to VS Code** — the push finishes back in VS Code, not the browser.
   - If push still fails with "Permission denied" or nothing happens, see `git_troubleshooting_decision_tree.md` → *"Permission denied / 401 Unauthorized"*, or ask an instructor.

✅ Go to your GitHub repository and refresh the page — you should see `notes.txt` there!

> 🏃 **Finished early?** Add a second file (e.g. `about-me.txt`), then stage, commit, and push it too. In the VS Code terminal, try `git log --oneline` to see your commit history.
>
> **Instructor note:** learners move at very different speeds here. Watch for anyone silently stuck — a stalled clone or failed push is easy to hide. Circulate rather than waiting for hands.

---

## 💻 Exercise B: Make Changes, Stay in Sync & Resolve a Conflict (30 mins)

*Goal: Edit your file, commit the change, and practice pulling updates from GitHub.*

### Part 1 — Edit a File and Push Again

1. Open `notes.txt` in VS Code.
2. Add a new line:
   ```
   Day 2: Stage → Commit → Push is the core workflow!
   ```
3. Save the file.
4. Go to **Source Control**, stage the change (**+**), commit with a message like `Add Day 2 notes`, and then push (Sync Changes).

✅ Check GitHub — your new line should be there.

### Part 2 — Edit Directly on GitHub (Simulating a Teammate's Change)

Sometimes a colleague (or your future self on another computer) will make a change on GitHub directly. Let's simulate that:

1. Go to your GitHub repository.
2. Click on `README.md`.
3. Click the **pencil icon** ✏️ (Edit this file) at the top right.
4. Add a line at the bottom:
   ```
   Updated from GitHub directly!
   ```
5. Scroll down and click **Commit changes** → then **Commit changes** again in the dialog.

✅ Now GitHub has a newer version than your local copy.

### Part 3 — Pull the Changes to Your Computer

1. Go back to VS Code.
2. Click the **Sync Changes** button at the bottom (or `Ctrl+Shift+P` → **Git: Pull**).
3. Open `README.md` in VS Code — you should see the line you added on GitHub.

✅ Your local copy is now up to date. This is the **Pull** action — bringing the latest from GitHub to your computer.

### The Golden Rule

> **Always Pull before you Push.** When you work with others (or across multiple computers), always pull the latest changes before making your own. This avoids conflicts.

### Part 4 — Instructor Demo: When Pull Hits a Conflict (5 mins)

Sometimes the same line gets changed in two places before you can pull. Git can't guess which version you want — this is a **merge conflict**. Watch the instructor demo this on the class repo:

1. Edit the first line of `notes.txt` **on GitHub** (pencil icon → change the text → commit).
2. Edit the first line of `notes.txt` **in VS Code**, locally, to something different. Stage & commit it (don't push yet).
3. Click **Sync Changes** (this pulls first) — VS Code reports a conflict, and `notes.txt` now shows conflict markers:
   ```
   <<<<<<< HEAD
   your local version of the line
   =======
   the version from GitHub
   >>>>>>> origin/main
   ```
4. Delete the version you don't want, and delete the `<<<<<<<`, `=======`, `>>>>>>>` marker lines — or click the **Accept Current/Incoming/Both** buttons VS Code shows above the conflict.
5. Save, **Stage**, **Commit** (message like `Resolve conflict in notes.txt`), then **Push**.

> 💡 **A conflict isn't an error — it's Git asking you to decide.** Your work is never lost; it's sitting right there in the markers, waiting for you to choose. See `git_troubleshooting_decision_tree.md` for a written walkthrough of this if you hit one on your own later.

---

## 👥 Exercise C: Pair Collaboration (15 mins)

*Goal: Practice collaborating with a partner on the same repository, without branches — just the Pull → Edit → Stage → Commit → Push loop you already know.*

Pair up with one classmate. One of you is the **Repo Owner**, the other is the **Collaborator**. *(Odd number in class? Make one group of three — one Owner, two Collaborators.)*

> **Instructor note:** pair a confident learner with a slower one — in a pair, one broken setup blocks *both* people. Also: collaborator invites arrive by email/notification and can lag a minute or two; send them at the very start of this exercise so acceptance isn't the bottleneck.

### Step 1 — Owner: Create the Repo & Add Collaborator

1. Owner creates a **new public repository** on GitHub (e.g. `pair-practice-repo`), with a README.
2. Go to **Settings** → **Collaborators** → **Add people** → invite your partner by GitHub username or email.

### Step 2 — Collaborator: Accept & Clone

1. Collaborator accepts the invite (check email or GitHub notifications).
2. Clone the repo in VS Code (`Ctrl+Shift+P` → **Git: Clone**).

### Step 3 — Both: Pull, Edit, Push (take turns)

1. Both of you **Pull** first to make sure you're starting from the latest version.
2. Each person edits a **different file** (e.g. Owner edits `notes.txt`, Collaborator creates `partner-notes.txt`) so you don't collide.
3. Stage → Commit → Push your change.
4. Before your next push, always **Pull** first — practice the Golden Rule from Exercise B.

✅ Check GitHub together — you should both see each other's commits in the repo's history.

> ⚔️ **Hit a merge conflict?** Congratulations — you've just recreated the exact scenario from Exercise B Part 4, live. This is a bonus, not an accident. Resolve it together: open the file, pick which version to keep (or combine both), delete the `<<<<<<<` / `=======` / `>>>>>>>` marker lines, then Save → Stage → Commit → Push. The written walkthrough is in `git_troubleshooting_decision_tree.md`.

> 💡 Ready for more? `assignment.md` has an optional **Exercise C2** where you'll add branches and Pull Requests on top of this same workflow.

---

## 📘 Module 3: What is Google Colab? (10 mins) — Optional

### Overview

**Google Colab** (short for Colaboratory) is a free tool from Google that lets you write and run Python code in your browser — no installation needed.

Think of it as a notebook where each "cell" can contain either text or runnable code. It's widely used in data science because:

- **No setup required** — just open your browser and start coding
- **Free computing power** — Google provides free access to fast processors (GPUs)
- **Easy sharing** — share a link like a Google Doc
- **Connects to GitHub** — you can save your Colab notebooks directly to your GitHub repository

### How Colab Connects to GitHub

You can save a Colab notebook to GitHub in two clicks:

1. In Colab: **File** → **Save a copy in GitHub**
2. Choose your repository and branch, write a commit message, click **OK**

Your notebook (`.ipynb` file) will appear in your GitHub repository — just like any other file.

### Try It (If Time Allows)

1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Click **New Notebook**
3. In the first cell, type:
   ```python
   print("Hello from Colab!")
   ```
4. Run it with **Shift + Enter**
5. Go to **File** → **Save a copy in GitHub** → select `my-learning-journal` → write a commit message → click **OK**
   - 💡 The first time, Colab asks to **authorize GitHub** — this is a *separate* permission from the one you gave VS Code. Click **Authorize** in the popup and continue.
6. Refresh your GitHub repository — the `.ipynb` file should be there!

---

## ✅ Can You Do This? (Self-Check)

Before you leave, make sure you can answer YES to all of these:

- [ ] I can explain Git and GitHub to a friend in one sentence each
- [ ] I can explain the difference between "local" and "remote"
- [ ] I can create a repo on GitHub, clone it, and open it in VS Code
- [ ] I can stage a change, write a commit message, and push to GitHub
- [ ] I can pull the latest changes from GitHub to my computer
- [ ] I know what a merge conflict looks like and roughly how to resolve one

---

## 🎓 Wrap Up & Key Takeaways (included in Module 3 time)

You've covered the complete beginner workflow for Git and GitHub!

**What you learned:**

- **Git** tracks changes to your files like a time machine
- **GitHub** stores those changes in the cloud
- **Local** = your computer; **Remote** = GitHub
- The core workflow: **Stage → Commit → Push**
- To get the latest from GitHub: **Pull**
- **VS Code** makes all of this accessible without needing to memorise commands

**What to do next:**

- Use this workflow for your next project — even a simple one
- The more you practise, the more natural it feels
- Reference the `git_command_cheatsheet.md` whenever you need a reminder

> "The best way to learn Git is to use it. Start with one file, one commit, one push. You've already done that today." 🎉
