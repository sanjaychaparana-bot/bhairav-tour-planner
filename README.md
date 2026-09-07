# Bhairav Tour Planner

This repository contains a simple static MVP for Bhairav Tour Planner — a brochure website with sample packages, a custom tour request form, blog placeholders, FAQ, and contact form.

- Live repo: https://github.com/sanjaychaparana-bot/bhairav-tour-planner

## One-click Deploy to Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/sanjaychaparana-bot/bhairav-tour-planner)

Click the button above to start a new site on Netlify using this repository. You will be asked to sign in and authorize Netlify to access your GitHub account (or to select the repository). After authorization, Netlify will import the repository and create automatic deploys for the `main` branch.

Recommended Netlify settings (the repo already includes `netlify.toml`):
- Build command: (leave empty)
- Publish directory: `/` (root)
- Branch to deploy: `main`

After the initial deploy Netlify will give you a temporary `*.netlify.app` URL. From that Site dashboard you can add a custom domain later.

## Manual Deploy / Configure Automatic Deploys (if you prefer step-by-step)
1. Sign in to Netlify (https://app.netlify.com/) and click "Add new site" → "Import from Git".
2. Connect your GitHub account and allow access to this repository: `sanjaychaparana-bot/bhairav-tour-planner`.
3. Select the repository.
4. Build settings:
   - Build command: (leave empty)
   - Publish directory: `/`
5. Click "Deploy site". Netlify will create the site and start the first deploy.
6. In Site settings → Build & deploy → Continuous Deployment make sure "Deploy contexts" are enabled and `main` is set as the production branch.

## Post-deploy: Required changes
- Forms: Create forms on Formspree (https://formspree.io) and replace the placeholder action endpoints in the files:
  - `custom-tour.html` — replace `https://formspree.io/f/{your-id}` with your form endpoint
  - `contact.html` — replace `https://formspree.io/f/{your-id}` with your form endpoint
- Contact email: already set to `bhairavtourplanner@gmail.com` in `contact.html`.
- Images: Replace the Unsplash image URLs in `index.html` and `packages.html` with your own assets.
- Logo: Replace `assets/logo.svg` with your final logo file (SVG/PNG).

## Local preview
- Quick preview: open `index.html` in your browser.
- Better (local server):
  - Python 3: `python -m http.server 8000` then open http://localhost:8000

## Custom domain
1. Buy a domain from a registrar (Namecheap, Google Domains, GoDaddy, etc.).
2. In Netlify Site dashboard → Domain settings → Add custom domain.
3. Follow Netlify's DNS instructions — they will provide records to add at your registrar.
4. After DNS propagation Netlify will provision HTTPS automatically.

## Optional enhancements I can help with
- Replace Formspree IDs and test forms (share Formspree IDs or account access).
- Connect the repository to Netlify for you (you will need to sign in to Netlify and authorize access).
- Add a booking calendar integration (Calendly) or payment deposit flow (Stripe).
- Add Netlify Identity / Netlify CMS for editing packages and blog posts without code.
- Improve SEO with structured data and page-specific meta tags.

If you want, I can walk you through the Netlify authorization flow step-by-step and finish the setup while you sign in — tell me when you are ready to click the deploy button and I’ll guide you through each screen.