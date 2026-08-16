# Navya Mathur — Portfolio Website

A static, fixed-width (non-responsive) portfolio site built from the original PDF.

## Files
- `index.html` — the whole site (single page, fixed 1300px width)
- `images/` — all 16 portfolio spreads as JPGs, referenced by `index.html`

Keep these two together — don't separate the HTML file from the `images` folder.

## How to publish this on GitHub Pages

1. **Create a new repository** on GitHub (e.g. `navya-portfolio`). Keep it public (GitHub Pages needs a public repo unless you're on GitHub Pro/Team).

2. **Upload the files**:
   - Easiest way: on the repo page, click "Add file" → "Upload files", drag in `index.html` and the whole `images` folder, then commit.
   - Or via git from your terminal:
     ```
     git init
     git add .
     git commit -m "Add portfolio site"
     git branch -M main
     git remote add origin https://github.com/YOUR-USERNAME/navya-portfolio.git
     git push -u origin main
     ```

3. **Turn on GitHub Pages**:
   - Go to your repo's **Settings** → **Pages** (left sidebar).
   - Under "Build and deployment" → "Source", select **Deploy from a branch**.
   - Under "Branch", select **main** and folder **/ (root)**, then **Save**.

4. **Wait 1–2 minutes**, then refresh the Pages settings screen — it'll show your live URL, something like:
   `https://YOUR-USERNAME.github.io/navya-portfolio/`

That's it — no build step, no server needed, it's plain HTML.

## Editing later
- To swap an image, just replace the matching file in `images/` (keep the same filename) and re-upload.
- To change text overlays or add a contact/nav link, edit `index.html` directly — it's plain HTML/CSS, no dependencies.
