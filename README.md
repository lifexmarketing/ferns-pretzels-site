# Fern's Homemade Soft Pretzels — Website

Static website for Fern's Homemade Soft Pretzels at The Greater Bridgeton Amish Farm Market, 2 Cassidy Court, Bridgeton, NJ 08302.

This repository contains the **prebuilt static site** — plain HTML, CSS, JavaScript, and images. There is no build step required to deploy it.

## What's inside

- `index.html` — home page
- `privacy-policy/index.html` — privacy policy page
- `404.html` — fallback page (serves the home page for unknown URLs)
- `assets/` — compiled CSS and JavaScript
- `images/` — photos and logo
- `robots.txt`, `sitemap.xml`, `llms.txt`, `favicon.png`, `opengraph.jpg`

## Deploy to Cloudflare Pages (checklist)

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com) and go to **Workers & Pages → Create → Pages**.
2. Choose **Connect to Git** and select this GitHub repository (`ferns-pretzels-site`).
3. On the build settings screen:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (the repository root)
4. Click **Save and Deploy**. The first deploy takes about a minute.
5. Your site will be live at `https://<project-name>.pages.dev`.
6. *(Optional)* Add a custom domain: in the Pages project, open **Custom domains → Set up a custom domain** and follow the DNS instructions.

Every push to the `main` branch of this repository automatically redeploys the site.

## Updating the site

The site is maintained in a Replit project (React + Tailwind CSS). To update:

1. Edit the site in Replit.
2. Rebuild and push the new static output to this repository's `main` branch.
3. Cloudflare Pages redeploys automatically.
