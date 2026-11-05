# Sinha Homes – final website

The production-ready website source is maintained in `index.html`.

## Technology
- HTML5
- CSS3 (embedded in the HTML file)
- Vanilla JavaScript (embedded in the HTML file)
- Three.js r128 for the scroll-driven 3D house-building hero scene
- Google Fonts for typography

## Preview locally
Open `index.html` in a modern browser. An internet connection is required for the external Three.js and Google Fonts libraries and any externally hosted image assets.

## Deployment
Upload `index.html` to the document root of the target domain or subdomain using cPanel File Manager or FTP. Ensure it is named `index.html`.

## Before publishing
- Test the page on desktop and mobile browsers.
- Verify telephone, WhatsApp and email contact details.
- Confirm that all referenced image assets and external libraries load correctly.
- Test the English/Sinhala language switch, navigation, house model pages, cost estimator and enquiry flows.
- Confirm that the scroll-based 3D hero works on target mobile devices and that its fallback presentation is acceptable when WebGL is unavailable.

The HTML includes the page styling and application scripts. No separate `styles.css` or `script.js` files are required.


## SEO and Google Search setup

The official indexing domain is `https://www.sinhahomes.lk/`.

The repository now includes crawlable section URLs and page-specific metadata:
- `/about/`
- `/services/`
- `/house-designs/`
- `/projects/`
- `/why-choose-us/`
- `/cost-estimator/`
- `/contact/`

SEO files:
- `robots.txt` allows crawling and points search engines to the sitemap.
- `sitemap.xml` lists the homepage and the main section pages.
- `.htaccess` redirects requests to HTTPS and the official www hostname, and supports application routes on Apache hosting.
- Each section directory contains its own `index.html` with a page-specific title, description, canonical URL and WebPage structured data.

## Deployment requirements

Upload the complete repository contents to the document root for `www.sinhahomes.lk`, preserving the section folders and filenames. Do not upload only the root `index.html`.

The included `.htaccess` is for Apache hosting (commonly used with cPanel). If the hosting server uses Nginx or another platform, configure equivalent HTTPS/www redirects and route handling in that platform instead.

After deployment:
1. Open each section URL directly and confirm it loads after a refresh.
2. Check `https://www.sinhahomes.lk/robots.txt` and `https://www.sinhahomes.lk/sitemap.xml`.
3. Add and verify the Domain property `sinhahomes.lk` in Google Search Console.
4. Submit the sitemap URL: `https://www.sinhahomes.lk/sitemap.xml`.
5. Use URL Inspection to request indexing for the homepage and important section pages.

Google controls crawling, indexing and sitelink display. A sitemap submission or URL inspection request does not guarantee inclusion or a particular sitelink layout.
