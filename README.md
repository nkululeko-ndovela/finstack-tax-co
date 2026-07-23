# Finstack Tax Co. — website

Two design directions for the Finstack Tax Co. site, both static HTML (no build step needed).

- `/v1` — ledger / forest-green editorial design
- `/v2` — stamped-receipt design, with a live click/visit tracker built in
- `/index.html` — a simple landing page linking to both

## Before going live

Both versions need one thing filled in to actually send contact-form emails:

1. Go to [web3forms.com](https://web3forms.com) and enter your email — no account needed.
2. They'll email you an access key.
3. In each `index.html`, find:
   ```html
   <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">
   ```
   and replace `YOUR_WEB3FORMS_ACCESS_KEY` with the key they send you.

## Hosting on GitHub Pages

1. Push this folder to a GitHub repository.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a branch," branch `main`, folder `/ (root)`.
4. Save. GitHub will give you a URL like `https://<username>.github.io/<repo-name>/`.
5. Give it a minute or two after each push for the Pages build to finish.

Once live:
- Landing page: `https://<username>.github.io/<repo-name>/`
- Version 1: `https://<username>.github.io/<repo-name>/v1/`
- Version 2: `https://<username>.github.io/<repo-name>/v2/`
