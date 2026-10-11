# DIDIT INTEL

Original, static OSINT resource directory. Free to host on GitHub Pages or Cloudflare Pages. No paid API, build system, tracking, or backend required.

## Start locally
Open `index.html` in a browser. Search, filter, save favorites, and import bookmarks. Imported links and favorites are stored in that browser's localStorage, **not synced across devices or committed to GitHub**. Export the full JSON library to preserve a portable copy.

## Deploy on GitHub Pages
1. Create a public repository named `didit-intel`.
2. Upload `index.html` and this README to the repository root.
3. In Settings > Pages, choose Deploy from a branch, `main`, `/ (root)`, and Save.
4. Your site will be at `https://YOUR_USERNAME.github.io/didit-intel/` after deployment.

## Deploy on Cloudflare Pages
Connect your GitHub repo via Workers & Pages > Create > Pages > Import an existing Git repository. Build command `exit 0`; output directory `/` (repository root) for this static-only project, or deploy the root folder using Direct Upload. Cloudflare will provide a `pages.dev` address. If the dashboard disallows `/` as output, use a `public` folder containing `index.html` and set output directory to `public`.

## OSINT4ALL import plan
Source: https://start.me/p/L1rEYQ/osint4all

1. Confirm whether the curator permits bulk reuse. Do not claim affiliation with or ownership of the original collection.
2. If the curator supplies an HTML bookmarks export, import it through the site's Import bookmarks dialog. start.me's official Data > Exports option is for **your own account/pages**, not a way to export someone else's public page.
3. Alternatively, collect publicly visible outbound links in a permission-compliant manner and prepare a Netscape bookmarks HTML or JSON file; do not bypass access restrictions or rate limits.
4. Deduplicate normalized HTTP(S) URLs, preserve category provenance where available, and audit links for redirects, malicious destinations, and dead pages.
5. Write original descriptions and source attribution; remove or restrict links that create privacy or misuse risks.
6. Save reviewed resources to a checked-in JSON data file in a later version so **all visitors** see the imported directory, rather than only the importing browser.

## Editorial and privacy notes
Seed entries are independently selected examples, **not extracted from OSINT4ALL**. Tools are provided for lawful research only. Never enter credentials or private information into untrusted third-party sites. Do not scrape personal data or evade access controls.

## Next iteration
Move resource catalog to `data/resources.json`, add admin review, dead-link validation and provenance labels, and add a JSON-based static build step. Current MVP intentionally avoids server-side infrastructure.
