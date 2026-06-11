# World Cup Story — Website

Static marketing + legal site for the **World Cup Story** game.
Plain HTML/CSS — no build step. Open `index.html` to preview locally.

```
index.html      Landing page
privacy.html    Privacy Policy   (use this URL for App Store / Google Play)
terms.html      Terms of Service
styles.css      Shared styling
CNAME           Custom domain for GitHub Pages
```

## Publish for free with GitHub Pages

1. Create a new GitHub repo, e.g. `world-cup-story-site`.
2. Upload all files in this folder to the repo root.
3. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main` / root, **Save**.
4. After ~1 minute your site is live at:
   `https://<your-username>.github.io/world-cup-story-site/`
   - Privacy Policy URL: `https://<your-username>.github.io/world-cup-story-site/privacy.html`
   - Use that URL in App Store Connect and Google Play Console.

## Point the custom domain (world-cup-storygame.com)

1. Buy the domain `world-cup-storygame.com` from a registrar (Namecheap, GoDaddy, etc.).
2. At the registrar's DNS settings, add:
   - Four `A` records for the apex domain → GitHub Pages IPs:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record `www` → `<your-username>.github.io`
3. In the repo **Settings → Pages → Custom domain**, enter `world-cup-storygame.com`
   (the included `CNAME` file already sets this) and enable **Enforce HTTPS**.
4. After DNS propagates, the site is live at `https://world-cup-storygame.com`.

## Notes
- Update the contact email (currently `ertugrul_kurtul@hotmail.com`) if you prefer
  a different address — change it in all three HTML files.
- The Terms page includes a non-affiliation disclaimer; keep it for store review.
