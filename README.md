# Texas Triggers — Reaper Launch Email Preview

Static preview of the 10-email launch sequence for the Sig P320 "Reaper" FRT.
Tab between emails by number, or use the previous/next pager.

## Contents

- `index.html` — the preview page, all 10 emails inline
- `assets/` — logo and product images, served locally

## Deploying (Cloudflare Pages)

No build step. Point Cloudflare Pages at this repo:

- Build command: *(leave empty)*
- Build output directory: `/`

Then attach the subdomain under the project's **Custom domains** tab.

## Note on the email HTML

The page is self-contained and uses relative image paths, which is what a
hosted preview wants. Email clients cannot resolve relative paths — if the
email markup is lifted out of here and put into a sending platform, the
`assets/...` image sources have to be swapped back to absolute URLs.
