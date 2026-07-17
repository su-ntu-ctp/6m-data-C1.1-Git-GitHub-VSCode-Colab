## Before the Session — What to Set Up

Please complete these steps **before class**. It should take about 20–30 minutes. If you run into trouble, reach out to your instructor.

---

### 1. Create Accounts (Free)

- **GitHub account:** Sign up at [github.com](https://github.com) (choose the free plan)
  - After signing up, **verify your email** (GitHub sends a confirmation link) and log in once normally in your browser. A brand-new, never-verified account may hit extra security checks (captchas, confirmation prompts) right when you're trying to push in class.
- **Google account:** You likely already have one. If not, sign up at [accounts.google.com](https://accounts.google.com)

---

### 2. Install Software

#### Git
Git is the tool that tracks changes to your files.

- **Mac:** Open Terminal, type `git --version`. If Git is not installed, macOS will prompt you to install it automatically.
- **Windows:** Download from [git-scm.com/downloads](https://git-scm.com/downloads). Run the installer and accept all the default options.
  - **Windows + WSL users:** if you set up WSL (Windows Subsystem for Linux) in [Lesson 1.0 (Welcome & Onboarding)](../6m-data-1.0-Welcome-Onboarding/), open VS Code and click the blue "Open a Remote Window" button at the bottom-left → **Connect to WSL**. This gives you a small Linux workspace inside Windows, matching what we'll use in class.

To confirm Git is installed, open a terminal and type:
```
git --version
```
You should see something like `git version 2.x.x`.

#### VS Code (Visual Studio Code)
VS Code is a free code editor with built-in Git support. We'll use it as the main tool in class.

Download from: [code.visualstudio.com](https://code.visualstudio.com)  
Install it like any other application on your computer.

---

### 3. Set Up Git with Your Name and Email

*This only needs to be done once.*

Open a terminal (on Mac: search for "Terminal"; on Windows: search for "Git Bash") and type these two commands, replacing the example text with your own name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Use the same email address you used to sign up for GitHub.

---

### 4. Sign in to GitHub inside VS Code ahead of time

*This saves you a hiccup during class.*

1. Open **VS Code**.
2. Click the **account icon** (the little circle at the bottom-left of the window).
3. Choose **Sign in with GitHub**.
4. A browser window will open — click the green **Authorize** button and return to VS Code.

Think of it like logging into Gmail once so it remembers you — your first "push" in class won't stop to ask who you are.

---

### 5. Watch This Short Video (Recommended)

[Git & GitHub Zero to Hero](https://youtu.be/1I79WAZ4uSU) — about 15 minutes

This gives you a visual introduction to Git before class. Don't worry if not everything makes sense yet — we'll cover it all together.

---

### 6. Optional: Install the "Open in Colab" Chrome Extension

If you use Google Chrome, you can install this extension to open notebooks from GitHub directly in Google Colab:

[Open in Colab – Chrome Extension](https://chromewebstore.google.com/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo)

This is optional and only relevant if we have time to cover the Colab section.

---

### What You Do NOT Need

- You **do not** need to know how to code
- You **do not** need to know any terminal commands before class
- You **do not** need to install Python or any data science tools

The session is designed for beginners. If you can use a web browser and save a file on your computer, you're ready.

---

### Checklist Before Class

- [ ] GitHub account created at github.com
- [ ] Git installed (`git --version` works in terminal)
- [ ] VS Code installed and opens on your computer
- [ ] Git configured with your name and email
- [ ] Signed in to GitHub inside VS Code (account icon, bottom-left)
- [ ] Watched the intro video *(recommended)*
