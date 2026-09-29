# Karakol Tourist Guide

Static info board for guests — activities, transport, contacts, and prices around Karakol (Sep–Oct).

Live site (after you enable GitHub Pages): `https://abdelski.github.io/karakol-tourist-guide/`

## Deploy on GitHub Pages

### 1. Create the repo on GitHub

1. Go to [github.com/new](https://github.com/new)
2. Repository name: **`karakol-tourist-guide`** (must match for the URL above)
3. Public repository
4. Do **not** add README, .gitignore, or license (this folder already has them)
5. Click **Create repository**

### 2. Push this folder

```bash
cd ~/Desktop/karakol-tourist-guide

git init
git add index.html README.md
git commit -m "Add Karakol guest info board for GitHub Pages"

git branch -M main
git remote add origin https://github.com/abdelski/karakol-tourist-guide.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Open `https://github.com/abdelski/karakol-tourist-guide`
2. **Settings** → **Pages** (left sidebar)
3. **Build and deployment** → Source: **Deploy from a branch**
4. Branch: **`main`** · Folder: **`/ (root)`**
5. **Save**

After 1–3 minutes the site is live at:

**https://abdelski.github.io/karakol-tourist-guide/**

### 4. Updates later

Edit `index.html`, then:

```bash
cd ~/Desktop/karakol-tourist-guide
git add index.html
git commit -m "Update guide content"
git push
```

Changes appear on the live site within a few minutes.

## Optional: custom domain

In repo **Settings → Pages → Custom domain**, add e.g. `guide.yourguesthouse.com` and set a CNAME record at your DNS provider.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Full guest information board (single page, no build step) |
