# Henry Dangerfield - Organist Website

Personal website for Henry Dangerfield - pipe organist.

## Deployment & Favicon Validation Checklist

After pushing changes to GitHub (especially favicon updates):

1. **Verify asset availability** (all should return 200):
   - `https://henrydangerfield.com/`
   - `https://henrydangerfield.com/favicon.ico`
   - `https://henrydangerfield.com/favicon-48.png`
   - `https://henrydangerfield.com/site.webmanifest`
   - `https://henrydangerfield.com/apple-touch-icon.png`

2. **Google Search Console**:
   - Verify correct property type is active (Domain property for `henrydangerfield.com`)
   - Use URL Inspection tool on homepage
   - Request reindex via "Request Indexing" button
   - Check for crawl errors or warnings

3. **Bing Webmaster Tools**:
   - Site verified via `msvalidate.01` meta tag in `index.html`
   - Use URL Inspection to check homepage indexing status
   - Submit URL for recrawl if needed
   - Monitor for crawl errors in Site Explorer
   - Note: Bing favicon updates also cache-lagged, typically 1–3 weeks

4. **Wait for SERP favicon update**:
   - Favicon changes in Google search results typically take **1–4 weeks** after recrawl
   - Google caches favicons aggressively; technical correctness ≠ immediate display
   - Monitor search results periodically; avoid repeated reindex requests

5. **Optional validation tools**:
   - [Google Rich Results Test](https://search.google.com/test/rich-results)
   - Browser DevTools Network tab to confirm 200 responses and correct MIME types
   - Test on mobile and desktop search

## Tech Stack

- Static HTML/CSS
- Hosted on GitHub Pages
- Custom domain via CNAME: `henrydangerfield.com`

## File Structure

- `index.html` – Homepage with biography
- `media.html` – Performance videos
- `style.css` – Site styles
- `sitemap.xml` – Search engine sitemap
- `robots.txt` – Crawler directives
- `site.webmanifest` – PWA manifest for mobile add-to-homescreen
- `favicon-*.png`, `favicon.ico`, `apple-touch-icon.png` – Icon assets
