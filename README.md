# gatesidemobility.com

Static website for GateSide Mobility. Plain HTML and CSS, no build step.

## Files
- `index.html` – the page (Home, Services, Why us, About, Contact)
- `styles.css` – all styling
- `logo.svg`, `mark.svg` – logo files (mark is also the favicon)
- `apple-touch-icon.png`, `og-image.png` – phone home-screen icon and link-preview image

## Edit locally
Open the folder in VS Code and open `index.html` in a browser (or use the Live Server extension).

## Deploy on GitHub Pages
1. Create a new public repo on GitHub (e.g. `gatesidemobility-site`) and push this folder to the `main` branch.
2. In the repo: Settings > Pages > Source: "Deploy from a branch", Branch: `main`, folder `/ (root)`.
3. Under Custom domain, enter `www.gatesidemobility.com`, save, and tick "Enforce HTTPS" once it becomes available.

## DNS (wherever gatesidemobility.com is managed)
- CNAME record: host `www` -> `<your-github-username>.github.io`
- A records for the bare domain (`@`), so gatesidemobility.com redirects to www:
  185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- Do NOT change the MX records. They keep Google Workspace email working.

DNS changes can take a few hours to take effect.
