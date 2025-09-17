# Simple GitHub Pages site

This repository contains a minimal static site for GitHub Pages using `index.html` and `site.css`.

How to publish on GitHub Pages

1. Create a new repository on GitHub. You can name it anything. For a user/organization site, name it `<username>.github.io`.
2. Push this folder's contents to the repository (master/main branch or a `gh-pages` branch).

Example commands (run in PowerShell):

```powershell
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

3. Open the repository on GitHub -> Settings -> Pages. Choose branch `main` (or `gh-pages`) and `/ (root)` folder. Save.
4. After a few minutes your site will be available at the provided URL (for user sites it's `https://<username>.github.io`).

Local preview

You can preview the site locally by opening `index.html` in your browser. For a slightly better dev experience run a simple static server. If you have Python installed:

```powershell
# Python 3
python -m http.server 8000
# then open http://localhost:8000
```

That's it — edit `index.html` and `site.css` to customize your page.