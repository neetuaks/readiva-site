# Readiva website

Static site for `https://readiva.wisdomveda.com`. Plain HTML and CSS, no build step, nothing loaded from other domains.

## Files
- `index.html` landing page
- `privacy.html`, `terms.html`, `disclaimer.html` legal pages. Paste your text where it says `<!-- PASTE LEGAL TEXT HERE -->`, then delete the sample sections and update the table of contents to match.
- `support.html` support and Grievance Officer details
- `styles.css` shared styles (light and dark mode)

## Fill in before launch
- Replace `[DATE]` on the three legal pages.
- Replace `[GRIEVANCE_OFFICER]` on `support.html`.
- When the apps are live, replace the two "Coming soon" store buttons on `index.html` with links to your listings, using the official badge artwork from Apple and Google.

## Deploy to GitHub Pages
1. Create a GitHub repository and upload these files at the root.
2. Add a file named `CNAME` at the root containing one line: `readiva.wisdomveda.com`
3. In the repository, open Settings, then Pages. Under Build and deployment choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. At your DNS provider for wisdomveda.com, add a CNAME record: name `readiva`, value `<your-github-username>.github.io`.
5. Back in Settings, Pages, enter `readiva.wisdomveda.com` as the custom domain and, once the DNS check passes, tick "Enforce HTTPS".

DNS changes can take from a few minutes to a few hours.

## Cloudflare Pages (alternative)
Create a Pages project from the repository with no build command and the root as the output directory. Then add `readiva.wisdomveda.com` under Custom domains.

## Privacy check
The pages make no requests to other domains: no fonts, scripts, analytics, embeds or cookie banner. Please keep it that way.
