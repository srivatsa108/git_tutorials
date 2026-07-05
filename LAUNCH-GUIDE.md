# 🚀 Launch Guide — Ship Your First GitHub Project

You're about to put a real, live website on the internet. Follow these in order. This uses everything from the mission — so it's also your first real push for real.

**You have three files to publish:**
- `index.html` — the guide itself (must be named exactly this)
- `README.md` — what people see on the repo page
- `LICENSE` — optional but nice (instructions in Step 6)

---

## Step 1 — Put the files in one folder

Make a folder on your computer called `operation-push-to-hq` and drop `index.html` and `README.md` into it. That folder is your project.

```bash
mkdir operation-push-to-hq
# move index.html and README.md into it, then:
cd operation-push-to-hq
```

## Step 2 — Reserve the empty locker (Beat 02)

Go to **github.com/new**:
- Name: `operation-push-to-hq`
- Visibility: **Public** ✅ (you want the world to see it)
- **Leave "Add a README / .gitignore / license" UNCHECKED** — you're bringing your own.

Create it, and keep the page open.

## Step 3 — Push it (Beats 04–09, for real this time)

```bash
git init
git status                 # sweep the room — nothing secret here, it's just a web page
git add .
git commit -m "Initial drop: interactive GitHub guide"
git remote add origin git@github.com:YOURUSERNAME/operation-push-to-hq.git
git branch -M main
git push -u origin main
```

Refresh your GitHub page — the files are live. **You've now shipped your first project.** 🎯

## Step 4 — Turn on GitHub Pages (make it a real website)

This is the magic step that renders your page instead of showing code:

1. In your repo, click **Settings** (top menu).
2. In the left sidebar, click **Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set branch to **main** and folder to **/ (root)**. Click **Save**.
5. Wait ~1 minute, then refresh. GitHub shows a green banner with your live URL:

   `https://YOURUSERNAME.github.io/operation-push-to-hq/`

Open it. Your illustrated, interactive guide is now public on the internet. 🌍

## Step 5 — Fix the link in your README

Your `README.md` has a placeholder link. Update it to your real URL so visitors can click straight through:

```bash
# edit README.md — replace YOURUSERNAME and the repo name in the live-guide link
git add README.md
git commit -m "Add live site link"
git push
```

Notice you just used the **standing orders** (add → commit → push). That's the daily loop for the rest of your GitHub life.

## Step 6 (optional) — Add a license so people can reuse it

On GitHub: click **Add file → Create new file**, name it `LICENSE`, and GitHub will offer a "Choose a license template" button — pick **MIT**, and it fills it in for you. Commit it. Done.

---

## Make it look sharp on your profile

- **Add a description + topics:** on the repo page, click the ⚙️ next to "About" and add a one-line description, your live URL, and topics like `git`, `github`, `tutorial`, `beginners`.
- **Pin it:** on your GitHub profile, click "Customize your pins" and pin this repo so it's the first thing visitors see.

---

## You're done — and look what you did

You didn't just publish a project. You published a project **that teaches the exact thing you just did.** When someone visits your live page and follows it to push *their* first repo, your first project did its job.

Welcome to GitHub, Agent. 🕵️
