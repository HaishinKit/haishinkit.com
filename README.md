# haishinkit.com

The HaishinKit landing page. Static HTML and CSS; no installation or build step required.

## Local preview

Serve this directory with a static HTTP server. The stylesheet and favicon use root-relative URLs, so preview through HTTP rather than opening the HTML file directly.

## GitHub Pages

1. Push these files to `main`.
2. In repository Settings → Pages, choose **Deploy from a branch**, `main`, `/ (root)`.
3. Set the custom domain to `haishinkit.com`. The tracked `CNAME` contains this domain.
4. Configure the domain's DNS for GitHub Pages using GitHub's current custom-domain instructions, then enable **Enforce HTTPS** when available.
5. After the domain is serving the site, submit `https://haishinkit.com/sitemap.xml` to Google Search Console and inspect the home URL.

Publishing and domain configuration are separate from adding the source files. No GitHub Actions workflow is needed.

## Content and search

- All navigation, SDK descriptions and FAQ answers are present in the initial HTML; no JavaScript is required.
- The canonical URL, Open Graph tags, sitemap and robots declaration use `https://haishinkit.com/`.
- JSON-LD describes the organization, website and three SDK source repositories. It reflects visible content and does not invent ratings or imply rich-result eligibility.
- Keep platform support and protocol maturity aligned with each SDK's README. Flutter development status and Swift WHIP/WHEP alpha status are stated explicitly.
- SDK versions and installation requirements are linked to their source repositories to avoid stale release numbers on this page.
- The hero graphic is an illustration of a streaming pipeline, not a functioning live stream or performance measurement.

Google Search's AI features use the same core SEO requirements as Search: crawlable pages, useful visible content and accurate metadata. Indexing, ranking and AI citations are not guaranteed. `llms.txt` is not required by Google for its AI search features.

References: [Google AI features](https://developers.google.com/search/docs/appearance/ai-features), [crawlable links](https://developers.google.com/search/docs/crawling-indexing/links-crawlable), [GitHub Pages custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
