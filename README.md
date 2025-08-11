# Portfolio — Deploy to GitHub Pages

This folder contains a single‑file portfolio with assets. The entry point is `index.html`.

## Quick deploy

1. Create a new GitHub repo (public), for example `username/portfolio`.
2. Push this folder's contents to the repo root.
3. Enable GitHub Pages:
   - Repo Settings → Pages → Source: Deploy from a branch
   - Branch: `main` (or `master`) → `/ (root)` → Save
4. Wait ~1–2 minutes. Your site will be at:
   - https://username.github.io/portfolio/

## Use a custom domain

1. In Settings → Pages → Custom domain, enter your domain (e.g., `www.example.com`). Save and enforce HTTPS.
2. Create DNS records at your domain registrar:
   - For apex/root (`example.com`), add A records:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - For `www` (recommended), add a CNAME pointing to `username.github.io`.
3. In your repo, create a file named `CNAME` (no extension) containing exactly your domain, e.g.:

```
www.example.com
```

4. Wait for DNS to propagate (can take minutes to hours). Then reload your site via your domain.

## Notes
- Keep file paths relative. Assets are in `Assets/...`.
- If you place the portfolio at the user site (username.github.io), put the files at the repo root of `username.github.io`.
  
