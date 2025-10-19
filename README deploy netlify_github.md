# The Baddie Habitat - Starter Site Package

This package contains a ready-to-deploy static website with:
- Home, Shop (10 product placeholders), About pages
- Simple client-side cart (localStorage)
- Toggleable Coming Soon & Under Construction flags (controlled by Netlify CMS / localStorage)
- Netlify CMS admin config (admin/config.yml) for content editing
- Placeholder product assets and logos

## Files
- index.html, shop.html, about.html
- css/style.css
- js/main.js, js/shop.js
- admin/ (Netlify CMS files)
- content/products (10 markdown product placeholders)
- site-settings.yml
- assets/ (placeholder images)

## How to deploy to GitHub + Netlify (step-by-step)

1. Create a new repository on GitHub named `thebaddiehabitat` (or any name you prefer).
2. Upload the contents of this package (all files & folders) to the repository root (you can drag-and-drop or use git).
   - Alternatively, you can `git init` locally and push to GitHub.
3. In Netlify:
   - Connect your Netlify account (you're already on Netlify). Click "New site from Git".
   - Choose GitHub and select the repository you created.
   - Set branch to `main` (or the branch you used).
   - Build command: leave blank (static site). Publish directory: `/` or leave default.
4. After deploy, go to `Site settings` → `Domain management` and confirm your Netlify domain or custom domain (thebaddiehabitat.me).
   - Since you bought the domain from Netlify, the domain should connect automatically.
5. Enable Netlify Identity + Git Gateway to use Netlify CMS (optional):
   - In Netlify dashboard, go to `Identity` and enable it.
   - Under `Identity` > `Services`, enable Git Gateway and follow instructions to create an access token.
6. (Optional) Enable Netlify Analytics or add Google Analytics:
   - For Google Analytics, add your GA tracking ID in the <head> of your pages.
7. Stripe setup (payments):
   - This starter site contains client-side cart only. To accept real payments you will need to create a small server endpoint that creates Stripe Checkout Sessions (server-side) and returns the session ID.
   - For quick testing, you can use Stripe test keys. For production, add your live keys in the server.
   - Netlify Functions (serverless) can host the checkout endpoint. See Stripe + Netlify examples: https://stripe.com/docs/checkout/integration-builder
   - We included an alert that notifies you that Stripe integration is required. When you're ready, I can generate the serverless function code for Netlify that connects to Stripe.

## Editing content with Netlify CMS
- Open `/admin/` on your deployed site (e.g., https://thebaddiehabitat.netlify.app/admin/).
- Log in via Netlify Identity (enable Identity + Git Gateway in Netlify Dashboard first).
- From the CMS you can edit pages, add products, change settings (Coming Soon / Under Construction / Launch Date).

## Next steps I can help with (choose one)
- Generate Netlify Function code (serverless) to connect to Stripe Checkout (I can produce ready-to-deploy function code).
- Install Netlify Identity + Git Gateway step-by-step and test CMS login.
- Replace placeholders with your real logos/images (you can upload them via the CMS).
- Customize the copy to be baddie-captivating (I can write the homepage & product descriptions).

--- END README
