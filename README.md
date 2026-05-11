# Inspectley App Store Pages

Static GitHub Pages site providing the Privacy Policy and Support URLs required for App Store Connect.

## Files

| File | Purpose |
|------|---------|
| `index.html` | App landing page |
| `privacy.html` | Privacy Policy |
| `support.html` | Support page |
| `style.css` | Shared stylesheet |

---

## Publishing to GitHub Pages

### Step 1 — Create a new GitHub repository

Go to [github.com/new](https://github.com/new) and create a **public** repository.

Suggested name: `inspectley-appstore-pages`

Do **not** initialize with a README (you already have one).

### Step 2 — Push this folder to GitHub

Replace `USERNAME` and `REPO` with your GitHub username and the repo name you chose.

```bash
cd /path/to/inspectley-appstore-pages

git init
git add .
git commit -m "Initial commit: Inspectley App Store pages"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repository on GitHub.
2. Click **Settings** → **Pages** (left sidebar).
3. Under **Source**, select **Deploy from a branch**.
4. Set Branch to `main` and folder to `/ (root)`.
5. Click **Save**.

GitHub will show a banner: *"Your site is live at https://USERNAME.github.io/REPO/"*

It may take 1–3 minutes to go live.

---

## Your Live URLs

After publishing, your pages will be at:

| Page | URL |
|------|-----|
| Privacy Policy | `https://USERNAME.github.io/REPO/privacy.html` |
| Support | `https://USERNAME.github.io/REPO/support.html` |

Replace `USERNAME` and `REPO` with your actual GitHub username and repository name.

---

## App Store Connect — Where to Paste

In **App Store Connect → App Information**:

| Field | URL to paste |
|-------|-------------|
| **Privacy Policy URL** | `https://USERNAME.github.io/REPO/privacy.html` |
| **Support URL** | `https://USERNAME.github.io/REPO/support.html` |

---

## Optional — GitHub CLI (if already authenticated)

If you have `gh` installed and are logged in:

```bash
cd /path/to/inspectley-appstore-pages
git init && git add . && git commit -m "Initial commit: Inspectley App Store pages"
gh repo create inspectley-appstore-pages --public --source=. --remote=origin --push
```

Then enable Pages via the GitHub website (Settings → Pages) — the CLI does not enable Pages automatically.
