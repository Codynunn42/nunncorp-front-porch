
NUNN CORPORATION — FRONT PORCH SITE
===================================

This folder contains a single-page, SEO-ready site for nunncorporation.com.
It’s designed to be public-facing, low-maintenance, and safe.

FILES
-----
- index.html         The site (edit text as needed)
- logo.svg           Placeholder logo (replace if you have a brand mark)
- cody.jpg           Placeholder — replace with Cody's photo
- og-image.png       Social share image used by X/LinkedIn/etc.
- robots.txt         Tells search engines to index the site
- sitemap.xml        Helps Google index faster
- favicon.ico        Small icon in the browser tab

QUICK EDITS (Optional)
----------------------
1) Replace /cody.jpg with a real photo (same filename).
2) If you have a brand logo, replace /logo.svg (or change <img src> in index.html).
3) Update the contact email in the “Contact” block inside index.html.

DEPLOY — NETLIFY (Free, recommended)
------------------------------------
1) Go to https://app.netlify.com and create/sign in to your account.
2) Click “Add new site” → “Deploy manually” and drag-drop this entire folder.
3) After deploy, Netlify will give you a temporary URL like https://<site>.netlify.app

CONNECT YOUR DOMAIN (Namecheap → Netlify)
-----------------------------------------
1) In Netlify → Site settings → Domain management → “Add custom domain”.
   Enter: nunncorporation.com (and also add www.nunncorporation.com)
   Netlify will show the exact DNS records you need.

2) In Namecheap:
   - Go to Dashboard → Domain List → nunncorporation.com → “Manage” → “Advanced DNS”.
   - Create/Update the following host records (use what Netlify shows you):
     • CNAME  | Host: www   | Value: <your-site>.netlify.app | TTL: Automatic
     • A/ALIAS| Host: @     | Value: (the A records Netlify shows) | TTL: Automatic
       (If A records aren’t shown, set a URL Redirect from @ to https://www.nunncorporation.com using 301 Permanent.)

3) Back in Netlify:
   - Click “Verify DNS configuration” until it turns green.
   - Enable HTTPS → “Provision certificate” (Let’s Encrypt). Wait for the green lock.

SEARCH CONSOLE (Ask Google to index you)
----------------------------------------
1) Go to https://search.google.com/search-console/
2) Add property → URL prefix → https://www.nunncorporation.com/
3) Choose verification method “HTML tag” and copy the meta tag.
4) Open index.html and paste the tag where indicated in the <head> section.
5) Re-deploy the site (drag-drop again to Netlify).
6) In Search Console → URL Inspection → submit https://www.nunncorporation.com/ for indexing.

DONE — Tell people: “Google Nunn Corporation.”
----------------------------------------------

Notes
-----
• This is a static site — fast, secure, low maintenance.
• When you have email set up, update the contact address in index.html.
• Keep robots.txt and sitemap.xml as-is for best SEO results.

COMM
----
Sentinel AI by Cody Nunn | Nunn Cloud
