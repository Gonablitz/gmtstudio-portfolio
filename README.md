Deployment instructions

Quick local test

- Open `index.html` or `main.html` in a browser to preview locally.
- Or run a simple HTTP server in the project folder:

```bash
# Python 3
python -m http.server 8080
# Then open http://localhost:8080
```

Netlify (recommended, no account required for drag & drop)

1. Go to https://app.netlify.com/drop
2. Drag and drop this project folder (the folder containing `index.html` and `main.html`).
3. Netlify will publish a live URL instantly.

GitHub Pages

1. Create a new GitHub repo and push this project.
2. In the repository Settings -> Pages, set source to `main` branch (root) or `gh-pages` branch.
3. Ensure there's an `index.html` at the repository root (this repo already has one).

Notes about assets

- This project references several remote images/GIFs. I attempted to download them into `assets/images`, but the environment couldn't fetch them (network blocked).
- You can download assets locally and place them into `assets/images`, then update `main.html` to reference the local files.

If you want, I can:
- Retry downloading assets (may require you run the provided PowerShell locally),
- Patch `main.html` to use local asset paths after you provide the files, or
- Proceed to initialize a git repo and prepare a sample commit for you.
