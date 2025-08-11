# Library Browser — GitHub Pages

This repo hosts a single-page, client-side library browser that lets you filter by author, title, and language.
It’s 100% static and works on iOS Safari when served over HTTPS (e.g., GitHub Pages).

## Quick start

1. Create a new GitHub repo (public or private is fine).
2. Upload **index.html** and **static.html** from this folder.
3. In the repo: **Settings → Pages → Build and deployment**:
   - **Source**: *Deploy from a branch*
   - **Branch**: `main` (or `master`) and **Folder**: `/ (root)`
   - Save.
4. Wait ~30–60 seconds for the site to publish.
5. Your site will be at:
   - `https://<username>.github.io/<repo>/` (serves `index.html`)
   - `https://<username>.github.io/<repo>/static.html` (static fallback, no search)

### Notes
- The data is embedded directly in `index.html` (base64 JSON), so you don’t need extra files.
- If you ever update the CSV, just regenerate the HTML and replace `index.html`.
- The static fallback shows the entire list grouped A–Z but has no search (guaranteed to render anywhere).
