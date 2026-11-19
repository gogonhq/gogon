# gogon.io

The company website of Gogon, which builds Streamfiesta. It is plain static HTML and CSS, with no
build step, scripts, fonts or analytics.

## Files

- `index.html`: the company home page, with the product list, approach, company information and contact.
- `products/<name>/index.html`: one page per product (`products/streamfiesta/`).
- `privacy.html`: the privacy notice for this website only.
- `assets/`: the Gogon logo (`gogon-*.png`, from the gogonhq GitHub avatar) and each product's mark.
- `404.html`, `robots.txt`, `sitemap.xml`, `favicon-32.png`, `apple-touch-icon.png`, `styles.css`.
- `CNAME` and `.nojekyll`: GitHub Pages serves the site on gogon.io.

Gogon is the identity; each product keeps its own name and mark. To add a product:
1. Copy `products/streamfiesta/` to `products/<name>/` and rewrite it.
2. Add its mark to `assets/`.
3. Add a `product-card` to the list in `index.html`, and update or remove the "More to come" card.
4. Add it to the JSON-LD `brand` list, the company facts, the footer and `sitemap.xml`.

## Preview

```sh
python3 -m http.server 8765   # then open http://localhost:8765
```

## Company facts on the site

These appear in `index.html` (in the visible text and in the JSON-LD block) and in `privacy.html`.
Check them before going live:

- Legal name: Gogon SHPK
- Registered in: Albania (no city or street address is shown)
- Contact: contact@gogon.io (also the address for the AWS account and Activate application)
- "Independent, self-funded" (the About section)
- Streamfiesta status: "Preparing for launch". Change it when Streamfiesta launches.

## Rules for the content

- Describe only what Streamfiesta has built. A planned feature may be called planned, never shipped.
- Show no prices, commission or other business numbers.
- Make no claims of guaranteed completion, accredited credentials or compliance.
- Streamfiesta is market-neutral: Albania appears only as Gogon's company location.
