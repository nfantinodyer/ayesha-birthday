# Happy Birthday, Mom 🌸

A single-page birthday card website for Ayesha — emerald & gold, Pakistani-inspired
florals, an "open your card" animation, falling petals, framed photos of the
family's handwritten wishes, and a featured handwritten note. One HTML file,
no build step, loads fast on mobile data.

## Before sharing

1. **Add the handwritten wishes** — photograph each family member's handwritten
   wish and save them as `wishes/wish-1.jpg`, `wishes/wish-2.jpg`, … (up to
   `wish-8.jpg`; copy another `<figure class="wish-frame">` line in `index.html`
   for more). Each frame hides itself automatically until its image exists.
2. **Add the featured handwritten note** — save it as `note.jpg` in this folder
   (next to `index.html`). That section also hides itself until the file exists.

Keep every photo under ~500 KB so the page loads fast in Pakistan
(on a Mac: open in Preview → File → Export → JPEG, quality ~70%; or crop tightly
to just the paper). Natural daylight, shot from straight above, looks best.

## Deploy to GitHub Pages (free)

```bash
cd ayesha-birthday
gh repo create ayesha-birthday --public --source=. --push
```

Then on github.com: repo **Settings → Pages → Deploy from a branch → main / (root) → Save**.
A minute later the site is live at `https://<your-username>.github.io/ayesha-birthday/`.

GitHub Pages is accessible from Pakistan (it has never been blocked there).

## Optional: custom domain

A domain doesn't change accessibility — it's purely a prettier link. If you buy
one (e.g. on Cloudflare or Namecheap, ~$10/yr), add it under
**Settings → Pages → Custom domain** and point a CNAME record at
`<your-username>.github.io`.

## WhatsApp link preview

To get a nice preview card when the link is shared on WhatsApp, add an image
named `preview.jpg` to this folder, then uncomment the `og:image` meta tag in
`index.html` and set it to the full deployed URL of that image.
