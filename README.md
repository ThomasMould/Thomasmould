# Thomas Mould — GitHub Pages package

This is the replacement homepage for **https://thomasmould.com/**. It is ready to upload; no build, package installation, server, or application JavaScript is required. Open `index.html` to preview it locally; an internet connection loads the Google font.

## Publish

1. Keep a copy of your current website before replacing its files.
2. Extract the ZIP and copy its contents into the folder your GitHub Pages site publishes. Put `index.html` directly in that folder, not inside an extra enclosing folder. Include `styles.css`, `favicon.svg`, `robots.txt`, `sitemap.xml`, `CNAME`, and the hidden `.nojekyll` file.
3. In the repository's **Settings → Pages**, choose **Deploy from a branch**, select your publishing branch, and select the folder containing these files (`/ (root)` if uploaded to the repository root).
4. Set the custom domain to **thomasmould.com** and enable **Enforce HTTPS** once GitHub makes it available. If that domain already points to this same GitHub Pages site, keep the existing working DNS settings.
5. If moving the domain to a different GitHub Pages repository, configure the destination repository's custom domain before changing DNS. Follow [GitHub's custom-domain instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site). Configure `www` too if you use it; GitHub can then redirect it to the chosen apex domain.

The included `CNAME` is for branch-based publishing. If you use a custom GitHub Actions publishing workflow, configure the custom domain in Settings → Pages; GitHub does not use this file for Actions deployments.

## Search setup

- Page title and description identify Thomas Mould and his product-design work.
- The canonical URL, profile metadata, structured profile data, sitemap, and custom domain consistently use `https://thomasmould.com/`.
- All biography and experience content is present in the initial HTML and works without JavaScript.
- `robots.txt` permits crawling and points to the sitemap.
- Both contact links go to LinkedIn. There is no public email address or `mailto:` link.

After the replacement is live, confirm the homepage, `/robots.txt`, and `/sitemap.xml` load successfully. Verify ownership in [Google Search Console](https://search.google.com/search-console/about), submit `https://thomasmould.com/sitemap.xml`, and use URL Inspection to request indexing of the homepage. Validate the profile data with Google's [Rich Results Test](https://search.google.com/test/rich-results).

These changes support crawling and clear identification for searches such as “Thomas Mould” and “Thomas Mould product designer”. Google controls indexing and rankings; first place is not guaranteed. See [Google's SEO guidance](https://developers.google.com/search/docs/fundamentals/do-i-need-seo).

## Design and maintenance

The layout has a centred, capped desktop width, additional space between Products & research and Practice entries, and more room below the introduction. Mobile uses two columns with the name above them. Instrument Sans Regular 400 loads from Google Fonts.

Edit visible content and metadata in `index.html`; edit presentation in `styles.css`. Keep the structured profile data consistent with the visible biography. No Google Analytics or other tracking code is included in this package; the current thomasmould.com page's analytics snippet is not carried over.

This package does not itself change GitHub, domain settings, or the currently hosted website.
