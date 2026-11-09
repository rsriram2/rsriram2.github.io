# Research website files

Open `index.html` in a browser, or upload this folder to your hosting provider.

## Replace a figure placeholder

All figure placeholders are in `images/` and referenced from `index.html`.
Example:

    <img src="./images/ct-extraction.svg" ...>

To use a real image, put `ct-extraction.png` (or `.jpg`/`.webp`) in the `images` directory and change `ct-extraction.svg` to `ct-extraction.png` in `index.html`. Repeat for any entry.

The layout maintains the image aspect ratio automatically and displays the entire image without cropping. For multi-panel figures, export at sufficient resolution and avoid tiny labels.

## Other updates
- Confirm exact manuscript statuses before publishing.
- Add DOI/PDF or code links when available.
- Replace the CV PDF when you have a newer version.
- The design uses no external CSS or JS frameworks.


## Portrait and research-at-a-glance (Nov 2026 update)
- The top introduction now shows a circular 190 px portrait with a thin blue border (126 px on mobile). It currently uses `images/portrait-placeholder.svg`, not a real photograph.
- To add your headshot, save the image as `images/headshot.jpg` and change the `src` in `index.html` from `./images/portrait-placeholder.svg` to `./images/headshot.jpg`. The circle cropping is handled automatically by CSS (`object-fit: cover`).
- Research at a Glance now summarizes four areas of scientific contribution rather than listing dataset counts.
- Research/publication figure placeholders remain in `images/` and can be swapped for real figures by changing their image `src` paths.

## Presentation thumbnails (Nov 2026 update)
- Six presentation entries now have thumbnails in `images/presentation-*.svg`.
- Replace these SVGs with actual poster or slide thumbnails (PNG, JPG, WEBP), then update the matching `src` in `index.html`.
- The Stroke 2026 thumbnail links to its existing published abstract DOI.
- The other thumbnails deliberately remain non-clickable until you provide a verified conference page, abstract URL, poster PDF, or presentation recording. To enable one, replace `<div class="talk-figure">... </div>` with `<a class="talk-figure" href="YOUR_VERIFIED_URL" target="_blank" rel="noopener noreferrer">... </a>`.
- If your poster is available only as a local PDF, place it in the site folder and use a relative `href="./posters/your-poster.pdf"`.
- Keep the presentation order and publication statuses accurate. A poster is not assumed to exist for a coauthored accepted oral presentation.


## 2026-11 update
- Research experience now uses six equal-width cards (3 × 2 on desktop, 2 × 3 on tablets, single column on mobile).
- Added University of Miami Miller School of Medicine, Clinical Research Data Specialist, June 2023–present.
- Added a placeholder for the 2023 UltraNet POCUS presentation: `images/presentation-ultranet-2023.svg`. Replace it with your poster thumbnail. If an online abstract or poster URL becomes available, wrap the `.talk-figure` in an `<a href="YOUR_URL">` as for Stroke 2026. Do not link to an unverified page.
- Added three dated News cards. Review and update publication status as editorial decisions arrive.
- The bundled CV PDF is the previously supplied version; paste the separately provided LaTeX blocks into your CV source and recompile before replacing this PDF.
