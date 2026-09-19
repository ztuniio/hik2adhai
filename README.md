# Hik2Adhai Cafe — Website

A single self-contained page (`index.html`) — all styles, scripts, fonts and images are embedded in the file, so there's nothing else to configure.

## Deploy with GitHub Pages

1. Create a new GitHub repository (e.g. `hik2adhai-website`) and upload `index.html` to the root of the repo (keep the filename exactly `index.html`).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set **Branch** to `main` (or `master`) and folder to `/ (root)`, then **Save**.
5. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Custom domain (optional)

If you want to use your own domain (e.g. `hik2adhai.com`):
1. Add a `CNAME` file to the repo root containing just your domain name.
2. In your domain's DNS settings, point it at GitHub Pages (an `A` record to GitHub's IPs, or a `CNAME` record to `<your-username>.github.io` for a subdomain).
3. In **Settings → Pages**, enter the custom domain and enable **Enforce HTTPS** once it's verified.

## Editable placeholders in the code

A few spots are marked `<!-- EDIT: ... -->` in `index.html` and are worth revisiting later:
- The **contact form** is front-end only — connect it to Formspree, EmailJS, Firebase, Supabase, or your own API to actually receive messages.
- The **Reviews "View Reviews"** button currently links to a Google search for the cafe — swap in a direct Google review link once you have one.
- The **map** is a styled placeholder with a working "Open in Google Maps" button — swap in a live Google Maps embed if you'd like.
