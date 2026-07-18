## After the Session — Practice & Reflection

Great work today! The best way to make Git and GitHub feel natural is to keep using them. Here are some activities to help you practise.

---

### 1. Practise the Core Workflow (30 min)

Create a brand-new GitHub repository for a personal project — it can be anything! A journal, a list of ideas, notes from another class. The topic doesn't matter; the practice does.

Do this at least 3 times:
1. Create or edit a file in VS Code
2. Stage it (click the `+` in Source Control)
3. Write a clear commit message describing what you changed
4. Push to GitHub (Sync Changes)

Then go to GitHub and check that your commits appear in the repository's history.

**Goal:** Build muscle memory for Stage → Commit → Push.

---

### 2. Reflection Journal (15 min)

Write a short note (200 words or less) answering these two questions:

- "What is one thing about Git or GitHub that I now understand and could explain to a friend?"
- "What is one thing I'm still unsure about, and what is my plan to figure it out?"

You can write this directly in a `reflection.txt` file in your GitHub repository — good practice!

---

### 3. Explore GitHub (15 min)

Browse GitHub to see how other people use repositories:

- Search for a topic you're interested in (e.g., "data science", "recipes", "beginner projects")
- Look at a public repository: notice the file list, the commit history, and the README
- Try clicking "Commits" to see the history of changes — this is what your project will look like too

---

### 4. Optional: Try Google Colab with GitHub (20 min)

If we covered the Colab section in class:

1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Create a new notebook
3. Write something in a code cell (even just `print("Hello!")`)
4. Save it to your GitHub repository via **File → Save a copy in GitHub**
5. Check your GitHub repo — your notebook should appear as a `.ipynb` file

---

### 5. Optional: Exercise C2 — Branching & Pull Requests

*Builds on Exercise D (Branch & Pull Request) — this time with a partner, adding the **peer review** step. Goal: practice the branch → PR → review → merge workflow real teams use, where someone else reviews before merging.*

Same partner, same repo from class (or a new one — your choice).

1. **Collaborator:** create a new branch (e.g. `add-yourname-notes`).
2. Add or edit a file on that branch (e.g. add a line with your name to `README.md`).
3. Stage → Commit → Push the branch (not `main`).
4. On GitHub, open a **Pull Request** from your branch into `main`.
5. **Owner:** open the Pull Request, check the **Files changed** tab for quality (clear commit message, no broken content, follows instructions), then click **Merge pull request**.
6. Both: **Pull** on `main` afterwards so your local copy has the merged change.

> 💡 This mirrors real teamwork: collaborators don't push straight to `main` — they propose changes via PR, and the owner (or a reviewer) gate-keeps quality before merging.

---

### You're Ready for More

Once you're comfortable with the basics, here are optional next steps to explore on your own:

- **GitHub Desktop** — a visual app for managing Git without any command line
- **`.gitignore`** — telling Git which files to never track (e.g. secrets, temp files)

These are topics for a future session. For now, focus on getting the core workflow smooth.
