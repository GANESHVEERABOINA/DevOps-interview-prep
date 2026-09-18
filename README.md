# DevOps Interview Prep — GitHub Pages site

Your one-day DevOps interview prep guide, ready to host as a free website on GitHub Pages. It's a single `index.html` file — no build step, no dependencies to install.

## Fastest way — using only the GitHub website

1. Go to [github.com/new](https://github.com/new) and create a new repository, for example `devops-interview-prep`. Keep it **Public** (GitHub Pages needs a public repo unless you're on a paid plan).
2. On the empty repo page, click **"uploading an existing file"** and drag in `index.html` from this download. Commit the change.
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment" → "Source", choose **Deploy from a branch**.
5. Branch: `main`, Folder: `/ (root)` → **Save**.
6. Wait about a minute, then refresh the Pages settings — GitHub will show your live URL:
   `https://yourusername.github.io/devops-interview-prep/`

## Using git from the terminal

Since you've already practiced these commands, this will feel familiar:

```bash
git init
git add index.html
git commit -m "Add interview prep guide"
git branch -M main
git remote add origin https://github.com/yourusername/devops-interview-prep.git
git push -u origin main
```

Then enable Pages the same way: **Settings → Pages → Deploy from a branch → main → / (root) → Save**.

## Notes

- Everything lives in one `index.html` file, so there's nothing to build or configure.
- It loads two Google Fonts from the internet (Source Serif 4, IBM Plex Mono). If you're ever offline, it falls back to your system fonts and still works fine — nothing breaks.
- It's mobile-friendly, so once it's live you can open the link on your phone right before you walk into the interview.
- To update the content later, just edit `index.html` and push again (or re-upload it on the website) — GitHub Pages redeploys automatically within a minute or two.

Good luck on Saturday.
