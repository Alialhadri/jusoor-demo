# Push to github.com/Alialhadri/jusoor-demo

From this folder (`jusoor-demo`), run:

```bash
# 1. Create the repo on GitHub first (github.com/new → name: jusoor-demo → public → no README)

# 2. Initialise and push:
git init
git add .
git commit -m "Jusoor demo v3 — bilingual AR/EN, Raqeem-style UI, real trends, worklist, LTFU recall, methodology"
git branch -M main
git remote add origin https://github.com/Alialhadri/jusoor-demo.git
git push -u origin main
```

Or with GitHub CLI in one step (skips step 1):

```bash
git init && git add . && git commit -m "Jusoor demo v3"
gh repo create Alialhadri/jusoor-demo --public --source=. --remote=origin --push
```

## Enable GitHub Pages
Repo → **Settings → Pages → Source: Deploy from a branch → `main` → `/ (root)` → Save**

Live at: **https://alialhadri.github.io/jusoor-demo/**
