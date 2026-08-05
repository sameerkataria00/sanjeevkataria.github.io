# Sanjeev Kataria — Real Estate Website

A multi-page, responsive website for Sanjeev Kataria, Realtor® with Alta Realty Group CA, Inc. (Newport Beach, CA).

## Pages
- `index.html` — Home (hero, trust stats, about teaser, track record, areas served)
- `about.html` — Full bio, specialties, languages, track record, areas served
- `listings.html` — Featured listing cards + two embedded CRMLS IDX search widgets
- `testimonials.html` — Client testimonials and rating
- `contact.html` — Contact info and inquiry form

All pages share the same `styles.css` and `script.js`, and the same nav/footer.

## IDX embeds (listings.html)
Two CRMLS searches are embedded as iframes, each with a fallback "Open in New Window" button and note:
1. **Sanjeev's Listings** — `https://www.crmls.org/servlet/lDisplayListings?AGENT=OCKATASAN&LA=EN`
2. **General Property Search** — `https://www.crmls.org/servlet/lDisplayListings?LA=EN`

**Important:** I couldn't verify from this sandboxed environment whether CRMLS actually allows itself to be embedded in an iframe on a third-party site (some MLS systems block this for compliance reasons via `X-Frame-Options`). Once you publish, open `listings.html` in a real browser and check:
- If the search tools load and work inside the boxes — great, no action needed.
- If the boxes appear blank — CRMLS is blocking the embed. In that case, remove the `<iframe>` elements in `listings.html` and keep just the "Open in New Window" buttons as clickable cards. Let me know and I can make that change for you.

## Before you publish, personalize it
1. **Photo**: replace `assets/placeholder-headshot.svg` with a real photo (e.g. `assets/agent-photo.jpg`) and update the `src` on every `<img id="agentPhoto">` tag (in `index.html` and `about.html`).
2. **Listings**: swap the three sample listing cards in `listings.html` for real current/sold listings (photos + details).
3. **Testimonials**: two of the three testimonials in `testimonials.html` are sample placeholders — swap in real client reviews (with permission) to keep things accurate.
4. **Contact form**: the form currently just shows an alert on submit. Wire it up to a real service like Formspree, Netlify Forms, or a mailto backend so messages actually reach you.
5. Double check phone, email, office address, and DRE license number are current.

## Publishing to GitHub Pages
1. Create a new repository on GitHub (e.g. `sanjeev-kataria-website`), or use an existing one.
2. Upload these files (`index.html`, `about.html`, `listings.html`, `testimonials.html`, `contact.html`, `styles.css`, `script.js`, `assets/`) to the repository — either via the GitHub web upload UI or `git push`.
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", choose the `main` branch and `/ (root)` folder, then click **Save**.
5. GitHub will publish the site within a minute or two. If the repo is named `<username>.github.io`, it appears at `https://<username>.github.io/`; otherwise at `https://<username>.github.io/<repo-name>/`.
6. Optional: add a custom domain under Settings → Pages → Custom domain, and configure DNS with your registrar.
