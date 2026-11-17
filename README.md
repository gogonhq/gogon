# gogon.io

The company website of Gogon, which builds Streamfiesta. It is plain static HTML and CSS, with no
build step, scripts, fonts or analytics.

## Files

- `index.html`: the home page, with products (Streamfiesta), company information and contact.
- `privacy.html`: the privacy notice for this website only.
- `404.html`, `robots.txt`, `sitemap.xml`, `favicon.svg`, `styles.css`.

To add a product later, copy the `<article class="product">` block in `index.html`, then
remove the sentence saying that future products will be listed there.

## Preview

```sh
python3 -m http.server 8765   # then open http://localhost:8765
```

## Company facts on the site

These appear in `index.html` (in the visible text and in the JSON-LD block) and in `privacy.html`.
Check them before going live:

- Legal name: Gogon SHPK
- Registered in: Albania (no city or street address is shown)
- Contact: hello@gogon.io (the mailbox must exist and receive mail before going live)
- "Independent, self-funded" (the About section)
- Streamfiesta status: "Preparing for launch". Change it when Streamfiesta launches.

## Rules for the content

- Describe only what Streamfiesta has built. A planned feature may be called planned, never shipped.
- Show no prices, commission or other business numbers.
- Make no claims of guaranteed completion, accredited credentials or compliance.
- Streamfiesta is market-neutral: Albania appears only as Gogon's company location.
