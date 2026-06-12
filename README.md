# Happy Birthday, Ayesha 🌸

A single-page birthday card website — emerald & gold, Pakistani-inspired florals,
an "open your card" animation, falling petals, family wishes, and a framed
handwritten note. One HTML file, no build step, loads fast on mobile data.

## Before sharing

1. **Edit the wishes** — open `index.html`, find the `✏️ EDIT` comment in the
   "Wishes for you" section, and replace the placeholder names/messages.
   Copy a whole `<li class="wish">…</li>` block to add more wishes.
2. **Add the handwritten note** — save a photo/scan of it as `note.jpg` in this
   folder (next to `index.html`). The section hides itself automatically until
   the file exists. Keep it under ~500 KB so it loads fast in Pakistan
   (on a Mac: open in Preview → File → Export → JPEG, quality ~70%).

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
