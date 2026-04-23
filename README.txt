Michel Photography — Static Website Export
===========================================

Contents
--------
Michel Photography.html   Homepage (Work, Tournaments, About, Services, Contact)
saratoga-7s.html          Saratoga Sevens '25 — 30-frame dossier
og-image.png              1200×630 social share card
images/hero.jpeg          Hero image
images/saratoga/          30 tournament frames (webp)


Hosting
-------
Upload the contents of this folder to any static host
(Netlify, Vercel, Cloudflare Pages, GitHub Pages, S3, etc).

For clean URLs, set the default document to:
    Michel Photography.html

Or rename it to index.html before uploading:
    mv "Michel Photography.html" index.html

Then update the internal link in saratoga-7s.html:
    href="Michel Photography.html#..."  →  href="index.html#..."
    (or use "/#..." to link to the site root)


SEO / Social
------------
All meta tags (title, description, Open Graph, Twitter Card) reference:
    https://jamesmichelphotography.com/

If your final URL differs, update the <link rel="canonical"> and
og:url / twitter meta tags at the top of each HTML file.

The favicon is inline SVG (no separate file needed).
apple-touch-icon is set to og-image.png — replace with a 180×180
square if you want a proper app icon.


Contact info
------------
  Email:      hello@jamesmichelphotography.com
  Instagram:  @jamesmichelphotography

The contact form uses <form novalidate> — it does not submit anywhere.
Wire it to a real backend (Formspree, Basin, Netlify Forms, etc.)
by updating the action attribute and adding your endpoint.


Theme toggle
------------
The nav has a sun/moon button that flips between dark (noir) and
light (paper) mode. Selection persists in localStorage.
