# SystemR static review site

This folder is a self-contained, buildless static website for a public developer-app review page. It has no backend, database, login, forms, analytics, cookies, external scripts, or credentials.

## Local preview

From the repository root:

```text
python3 -m http.server 8000 --directory systemr_site
```

Open `http://127.0.0.1:8000/` locally, then stop the server when finished. No public exposure is required.

## GitHub Pages

1. Create or select a public repository approved by the human owner.
2. Copy the contents of `systemr_site/` to the repository root (or configure Pages to use this folder through the repository’s supported workflow).
3. Choose the publishing branch and root folder in GitHub Pages settings.
4. Confirm that `index.html`, `privacy.html`, `terms.html`, and `support.html` load over HTTPS.
5. Use the resulting public URL in the TikTok developer app only after human review.

## TikTok verification file

If TikTok later supplies a verification or signature filename, place that exact file at the exact path requested by TikTok in this folder, preserving its filename and contents. Do not invent a verification file. Re-run the static safety audit before publishing.

## Scope

The site explains a desktop creator workflow and does not claim automatic public publication. It does not include SystemR source code, local media, account identifiers, or integration credentials.
