# justembedme.com — website

Static marketing site for **JustEmbedMe** — a product of Joza Solutions LLC.

> Frontier open-source embeddings, hosted. The embeddings API you could run yourself — so you never have to.

## Stack

A single self-contained `index.html` — **no build step, no dependencies** (inline CSS plus one tiny vanilla-JS copy button). Edit it directly; what you commit is what ships.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The landing page |
| `404.html` | Branded not-found page |
| `og-image.png` | 1200×630 social preview image |
| `favicon.svg` | Site icon |
| `llms.txt` | Machine/agent-readable summary of the product |
| `robots.txt` / `sitemap.xml` | Crawl + SEO |
| `CNAME` | Custom domain (`justembedme.com`) |

## Deploy — Cloudflare Pages (recommended)

Cloudflare Pages serves from a **private** repo for free, which GitHub Pages does not.

1. Cloudflare → **Pages** → **Connect to Git** → select `justembedme/website`.
2. Framework preset: **None**. Build command: *(leave empty)*. Output directory: `/`.
3. Add custom domain **justembedme.com**.

> GitHub Pages also works, but serving from a private repo requires a paid GitHub plan (Pro/Team).

## Local preview

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

---

© Joza Solutions LLC. Not affiliated with, or endorsed by, the MTEB benchmark or its maintainers.
