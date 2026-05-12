# Pankaj Roy — Portfolio Website

A simple, single-file portfolio website built with HTML, CSS, and vanilla JavaScript.

## Files

- `index.html` — the entire site (HTML + CSS + JS embedded)

That's it. One file, no build step, no dependencies.

## Local preview

Just open `index.html` in your browser. Or run a local server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages — step by step

### Option A: Use a dedicated repo (cleanest)

1. **Create a new repository on GitHub** named `portfolio` (or anything you like).
2. **Clone it locally** and copy `index.html` into the folder:
   ```bash
   git clone https://github.com/Pankaj231123/portfolio.git
   cd portfolio
   # copy index.html into this folder
   git add index.html
   git commit -m "Add portfolio site"
   git push origin main
   ```
3. **Enable GitHub Pages**:
   - Go to your repo on GitHub → **Settings** → **Pages** (left sidebar).
   - Under "Build and deployment", set **Source** to **Deploy from a branch**.
   - Set **Branch** to `main` and folder to `/ (root)`.
   - Click **Save**.
4. **Wait 1–2 minutes**, then visit:
   `https://pankaj231123.github.io/portfolio/`

### Option B: Use your username repo (gets the cleanest URL)

This gives you `https://pankaj231123.github.io/` with no extra path.

1. Create a repo named **exactly** `Pankaj231123.github.io` (must match your GitHub username).
2. Push `index.html` to the `main` branch.
3. GitHub Pages is enabled automatically for username repos — no settings needed.
4. Visit `https://pankaj231123.github.io/` after 1–2 minutes.

### Updating the site later

Any time you push changes to the `main` branch, GitHub Pages rebuilds automatically.

```bash
# edit index.html
git add index.html
git commit -m "Update portfolio"
git push
```

## What to customize

- Update text content inside `index.html` directly — it's all readable HTML.
- Replace social links if needed (search for `github.com/Pankaj231123` and the LinkedIn URL).
- Add a custom domain later via Settings → Pages → Custom domain.

## Tech notes

- Fonts loaded from Google Fonts (Fraunces, Inter Tight, JetBrains Mono).
- Pure CSS animations + IntersectionObserver for scroll reveals.
- Fully responsive (mobile menu, fluid typography, grid breakpoints at 768px).
- No frameworks, no build tools, no npm install. Just open and use.