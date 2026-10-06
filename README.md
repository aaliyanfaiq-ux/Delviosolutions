# delviosolutions.com

Static landing page for Delvio Solutions Ltd, hosted on GitHub Pages.

## Before you publish — 3 edits in index.html
1. **Phone** — search `+44 0000 000000` and `tel:+440000000000`, replace both with your number.
2. **Contact form** — go to https://web3forms.com, enter your personal email, copy the access key it emails you, and replace `YOUR_WEB3FORMS_ACCESS_KEY`. Enquiries then land in that inbox; your email address never appears on the site.
3. **Centrion logo** — replace `assets/centrion-logo.svg` with your real logo (same name), or point the `<img src>` at e.g. `assets/centrion-logo.png`.

## Publish on GitHub Pages
1. github.com → New repository → name it `delviosolutions.com` → Public → Create.
2. "uploading an existing file" → drag in `index.html`, `CNAME`, `README.md` and the `assets` folder → Commit.
3. Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)` → Save.
4. Settings → Pages → Custom domain: `delviosolutions.com` → Save.

## DNS (at whoever holds the domain's DNS)
| Type  | Name | Value                    |
|-------|------|--------------------------|
| A     | @    | 185.199.108.153          |
| A     | @    | 185.199.109.153          |
| A     | @    | 185.199.110.153          |
| A     | @    | 185.199.111.153          |
| CNAME | www  | YOUR-GITHUB-USERNAME.github.io |

Delete any existing "parked" A/CNAME records for @ and www first. On Cloudflare, set these records to **DNS only** (grey cloud) until GitHub issues the certificate.

Once the domain check goes green (minutes to a few hours), tick **Enforce HTTPS** in Settings → Pages.

## Updating
Edit files on GitHub (pencil icon) or upload replacements — the site rebuilds automatically in about a minute.
