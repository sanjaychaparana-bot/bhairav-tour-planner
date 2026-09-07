# Bhairav Tour Planner

This repository contains a simple static MVP for Bhairav Tour Planner — a brochure website with sample packages, a custom tour request form, blog placeholders, FAQ, and contact form.

What is included

- index.html — Home / hero / featured packages
- packages.html — Package listing
- custom-tour.html — Custom itinerary request form (Formspree placeholder)
- blog.html — Blog / guides placeholder
- faq.html — Frequently asked questions
- contact.html — Contact form (Formspree placeholder)
- assets/logo.svg — Simple logo placeholder
- netlify.toml, _redirects — Netlify config

How to deploy (Netlify - recommended)

1. Sign in to Netlify and choose "Add new site" → "Import from Git".
2. Connect your GitHub account and select this repository: `sanjaychaparana-bot/bhairav-tour-planner`.
3. For a static site there is no build command. Set the Publish directory to `/` (root) and click "Deploy site".
4. After deploy, update your Formspree form IDs in `custom-tour.html` and `contact.html`.

How to configure forms

- We used Formspree placeholders: `https://formspree.io/f/{your-id}`. Create free forms at https://formspree.io and replace `{your-id}` with your form ID.

Custom domain (after you buy one)

1. In Netlify site dashboard → Domain settings → Add custom domain.
2. Point your registrar's DNS (A record or CNAME) to the Netlify-provided records. Netlify provides step-by-step instructions for common registrars.

Next recommended steps

- Replace images with your own photos in the `index.html` / `packages.html`.
- Replace logo.svg with a full logo from a designer.
- Add Google Analytics / privacy policy if needed.
- If you want, I can set up a Netlify automatic deploy preview and a one-click deploy button.

If you'd like, I can also:
- Wire up a simple booking calendar or payment integration.
- Add SEO-optimized blog posts and metadata.
- Configure Vercel instead of Netlify.

