# Full Snack Devs — Studio Website

## Quick Deploy to GitHub Pages

```bash
# 1. Create a new repo on GitHub called "fullsnackdevs.github.io"
# 2. Then run:
git init
git add .
git commit -m "Initial site launch"
git branch -M main
git remote add origin https://github.com/fullsnackdevs/fullsnackdevs.github.io.git
git push -u origin main
```

3. Go to **Settings → Pages** in the repo
4. Set source to **Deploy from a branch → main → / (root)**
5. Your site will be live at `https://fullsnackdevs.github.io`

## Before You Go Live — TODO

### Required
- [ ] **Careers form**: Sign up at [Formspree](https://formspree.io), create a form, and replace `YOUR_FORM_ID` in `index.html` (search for `formspree.io/f/YOUR_FORM_ID`)
- [ ] **Email addresses**: The site uses `support@fullsnackdevs.com` and `hello@fullsnackdevs.com`. Either set up these email addresses with your domain, or replace with a Gmail/personal email that works
- [ ] **Robert's LinkedIn**: Verify the LinkedIn URL for Bobby Groves in the Team section (currently `linkedin.com/in/bobbygroves` — update if different)
- [ ] **App Store links**: Replace the `#` placeholder hrefs on each app card with actual App Store URLs for Ninja Focus, Galaxy Glide, and Balloons: Skyward Quest

### Optional Enhancements
- [ ] **App icons**: Replace the colored letter placeholders in the belt and app cards with actual app icon images (drop PNGs into `/assets/` and update the `<div>` elements to `<img>` tags)
- [ ] **Team headshots**: Add photos to the team section (replace the initials-avatar divs with `<img>` tags)
- [ ] **Custom domain**: When you re-purchase `fullsnackdevs.io` (or pick a new domain), add a `CNAME` file containing the domain name to the repo root, then point your domain's DNS to GitHub Pages
- [ ] **Google Analytics**: If you want traffic tracking, add GA4 script to the `<head>` of all three HTML files
- [ ] **OG image**: Create a social share image and add `<meta property="og:image">` tags

## File Structure

```
├── index.html      ← Main landing page (all sections)
├── privacy.html    ← Privacy policy (link this in App Store Connect)
├── terms.html      ← Terms of service
├── style.css       ← Shared stylesheet
├── assets/         ← Drop app icons, team photos here
└── README.md       ← This file
```

## App Store Connect URLs

Once deployed, use these URLs in App Store Connect:

- **Support URL**: `https://fullsnackdevs.github.io/#contact`
- **Marketing URL**: `https://fullsnackdevs.github.io`
- **Privacy Policy URL**: `https://fullsnackdevs.github.io/privacy.html`
