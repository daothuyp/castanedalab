# Castañeda Lab website

A simple static site (HTML/CSS/JS, no build step) ready to host on GitHub Pages.

## Files
- `index.html` — home
- `research.html` — research overview
- `publications.html` — publication list
- `people.html` — PI and lab members
- `join.html` — open positions
- `contact.html` — contact info
- `css/style.css` — all styling
- `js/main.js` — mobile nav toggle

## Things to edit before you publish
- `people.html` — swap in your real roster, bios, and photos (drop an `<img>` into each `.avatar` div)
- `publications.html` — add your real publication list, or link out to Google Scholar / PubMed
- `contact.html` — replace the placeholder email
- Anywhere you see `20XX` or "replace with..." text

## Deploying to GitHub Pages

1. **Create a repository.** On GitHub, click "New repository." Name it whatever you like — if you name it `<your-username>.github.io`, the site will publish at the root of that URL; any other name publishes at `https://<your-username>.github.io/<repo-name>/`.

2. **Upload these files.** Either:
   - Drag-and-drop all files in this folder (keeping the `css/` and `js/` subfolders) into the GitHub web UI ("Add file" → "Upload files"), or
   - Push via git from your terminal:
     ```bash
     cd castaneda-lab-site
     git init
     git add .
     git commit -m "Initial site"
     git branch -M main
     git remote add origin https://github.com/<your-username>/<repo-name>.git
     git push -u origin main
     ```

3. **Turn on Pages.** In the repository, go to Settings → Pages. Under "Build and deployment," set Source to "Deploy from a branch," pick the `main` branch and `/ (root)` folder, then Save.

4. **Wait a minute, then visit your site.** GitHub will show the URL at the top of the Pages settings once it's live (usually `https://<your-username>.github.io/<repo-name>/`).

5. **Optional: custom domain.** If the lab has its own domain, add a `CNAME` file at the repo root containing just the domain name, and point the domain's DNS at GitHub Pages (GitHub's docs walk through the exact records).

Any time you edit a file and push to `main`, the live site updates automatically within a minute or two.
