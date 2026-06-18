# CoogieTech / Ozeed Website

This repository contains a single-page website (`index.html`) intended to be served at https://www.ozeed.com.

Quick deploy options (choose one):

1) GitHub Pages (recommended for simple static sites)

  - Create a GitHub repo and push these files to the `main` branch:

    ```bash
    git init
    git add .
    git commit -m "Initial site"
    git branch -M main
    git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
    git push -u origin main
    ```

  - The included GitHub Action (`.github/workflows/pages.yml`) will publish the site to the `gh-pages` branch on each push.
  - In the GitHub repository Settings → Pages, set the site source to the `gh-pages` branch (if needed). GitHub will serve the site at `https://YOUR-USERNAME.github.io/YOUR-REPO/`.
  - To use your custom domain `www.ozeed.com`, add a DNS CNAME record pointing `www` to `YOUR-USERNAME.github.io` and keep the `CNAME` file in the repo (present here).

2) Vercel or Netlify (automatic deploy + previews)

  - Sign up at https://vercel.com or https://app.netlify.com, connect your GitHub repo and deploy — both services auto-deploy on push and provide a shareable URL.
  - Add `www.ozeed.com` as a custom domain in the provider dashboard and follow their DNS instructions.

Notes on continued development and access:

- Keep developing locally and commit/push changes to `main`. Each push will trigger deploys (GitHub Action or your chosen provider) so your live site updates automatically.
- To retain the ability to improve the site while others use the link, use feature branches and pull requests to stage changes, or enable preview deploys (Netlify/Vercel provide these).
- Make backups and track changes with Git. If you want, I can create the GitHub repo for you (you must provide a GitHub token) or walk you through connecting your account.

If you want, I can also:
- Create the repository and push these files.
- Provide the exact DNS records for common registrars (GoDaddy, Namecheap, Cloudflare).
- Configure an SSL certificate (usually automatic on GitHub Pages / Vercel / Netlify).
