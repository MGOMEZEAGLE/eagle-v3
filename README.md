# Eagle Network Solutions — Website

Static marketing site. **No build step.** Plain HTML + CSS, with React/Babel and Google Fonts loaded from CDN and compiled in the browser. Deploys to Vercel as-is.

## Deploy to Vercel through GitHub
1. Create a new GitHub repository.
2. Upload everything in this folder to the repo **root** (so `index.html` and `vercel.json` sit at the top level, not inside a subfolder).
3. In Vercel: **Add New… → Project → Import** your repo.
4. Framework Preset: **Other**. Build Command: **empty**. Output Directory: **empty** (root). Deploy.

`vercel.json` handles clean URLs, pretty-path rewrites (e.g. `/cyber-insurance-readiness`, `/industries/municipalities`), and 301 redirects. Push changes to GitHub and Vercel redeploys automatically.

## Pages (19)
- `index.html` / `Homepage.html` — Home
- `Solutions.html` — Managed IT, Cybersecurity, Strategic IT, Hardware (tabs)
- `CoManagedIT.html`, `RemoteOnlyIT.html`, `CyberInsuranceReadiness.html`
- `Industries.html` hub + `Municipalities.html`, `Manufacturing.html`, `Distribution.html`, `ProfessionalServices.html`, `PropertyManagement.html`, `NonProfits.html`
- `About.html`, `Blog.html`, `Contact.html`
- `PrivacyPolicy.html`, `AccessibilityStatement.html`
- `sitemap.xml`, `robots.txt`

## Before launch (flagged placeholders)
- Replace image placeholders in `assets/` and descriptive photo captions with real photography.
- **TimeZest:** the scheduling embed uses a placeholder URL — swap in your real booking URL in `site/page.js` (the `schedule` builder).
- Confirm the LinkedIn/Instagram footer URLs and swap remaining placeholder team bios/blog content.
- The contact form and newsletter are front-end only. Wire them to your form handler / CRM.
