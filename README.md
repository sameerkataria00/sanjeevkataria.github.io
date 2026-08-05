# Sanjeev Kataria — Real Estate Website

A single-page, responsive website for Sanjeev Kataria, Realtor® with Alta Realty Group CA, Inc. (Newport Beach, CA).

## What's inside
- `index.html` — all page content and sections (hero, about, track record, listings, areas served, testimonials, contact, footer)
- `styles.css` — all styling
- `script.js` — mobile nav toggle, footer year, contact form placeholder handler
- `assets/placeholder-headshot.svg` — a placeholder graphic in place of a real headshot

## Before you publish, personalize it
1. **Photo**: replace `assets/placeholder-headshot.svg` with a real photo (e.g. `assets/agent-photo.jpg`) and update the `src` on the `<img id="agentPhoto">` tag in `index.html`.
2. **Listings**: swap the three sample listing cards in the `#listings` section for real current/sold listings (photos + details). Consider embedding an IDX/MLS widget from your brokerage for live listings.
3. **Testimonials**: two of the three testimonials are sample placeholders — swap in real client reviews (with permission) to keep things accurate.
4. **Contact form**: the form currently just shows an alert on submit. Wire it up to a real service like Formspree, Netlify Forms, or a mailto backend so messages actually reach you.
5. Double check phone, email, office address, and DRE license number are current.

## Publishing to GitHub Pages
1. Create a new repository on GitHub (e.g. `sanjeev-kataria-website`).
2. Upload these files (`index.html`, `styles.css`, `script.js`, `assets/`) to the repository — either via the GitHub web upload UI or `git push`.
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", choose the `main` branch and `/ (root)` folder, then click **Save**.
5. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.
6. Optional: add a custom domain under Settings → Pages → Custom domain, and configure DNS with your registrar.
