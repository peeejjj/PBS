# AkindaCo — Positive Behaviour Support website

A warm, single-page marketing website for **AkindaCo**, a Positive Behaviour Support (PBS)
practice for families with children and young people aged 2–18 (adult PBS too). Built with
plain HTML, CSS and a little JavaScript — no build step, no dependencies.

## Files

| File          | What it is                                          |
|---------------|-----------------------------------------------------|
| `index.html`  | All page content and structure                      |
| `styles.css`  | All styling (colours, layout, animation)            |
| `main.js`     | Small enhancements (menu, scroll reveals, form)     |
| `favicon.svg` | Browser-tab icon                                    |

## Preview it locally

Just double-click `index.html`, or from this folder run a tiny local server:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Content status

Everything on the page is real: Paula's bio (from akindaco.com), phone (08) 7081 5886,
Salisbury and North Adelaide locations, testimonials pulled from akindaco.com (Google
reviews), 2026–27 NDIS rate, brand colours/fonts/logo matching akindaco.com, and the
Calendly booking link (`https://calendly.com/akindaco/positive_behaviour_support`)
wired into every "Book your free 15-minute call" button.

The contact email `paula@akindaco.com` is already wired into the form.

## How the contact form works

By default the form opens the visitor's email app with a pre-filled message to
`paula@akindaco.com` — so it works with **no server required**. If you'd rather collect
enquiries automatically, point the form at a free service:

- **Formspree** — add `action="https://formspree.io/f/yourid" method="POST"` to the
  `<form>` in `index.html` and remove the mailto handler in `main.js`.
- **Netlify Forms** — add `netlify` to the `<form>` tag if you host on Netlify.

## Publishing (free options)

- **GitHub Pages** — push this repo, then enable Pages (Settings → Pages → Deploy from
  branch → `main` / root). Your site goes live at `https://<username>.github.io/<repo>/`.
- **Netlify / Cloudflare Pages** — drag-and-drop this folder, or connect the repo.

---

Colours, fonts and copy are all easy to adjust — the palette lives at the top of
`styles.css` under `:root`.
