# Nicholas Pfeil — Portfolio

Single-page static portfolio. Plain HTML + CSS, no JavaScript, no build step.

## Files

| File | Purpose |
|---|---|
| `index.html` | All content and structure |
| `style.css` | All styling (light + automatic dark mode) |
| `favicon.svg` | Browser-tab icon |
| `og-image.png` | 1200×630 link-preview cover (text-art map of the San Diego coast) |
| `resume.pdf` | **You add this.** Use a version *without* your phone number. |

## Preview locally

Double-click `index.html` to open it in your browser. All links are relative, so it works straight from disk.

Optional, closer to how Vercel serves it:

```powershell
python -m http.server 8000
```

Then open http://localhost:8000.

## Deploy to Vercel

1. Push this folder to a GitHub repository.
2. On vercel.com: **Add New → Project**, import the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty.
4. Click **Deploy**.

Every push to the `main` branch redeploys automatically.

## After the first deploy

Add your live URL to `index.html` (replace the TODO comment in `<head>`). Link previews (LinkedIn, iMessage, Slack) only show the cover image once these are full URLs:

```html
<meta property="og:url" content="https://YOUR-DOMAIN/">
<meta property="og:image" content="https://YOUR-DOMAIN/og-image.png">
```

LinkedIn caches previews. After changing them, refresh with the LinkedIn Post Inspector (linkedin.com/post-inspector).

## Updating content

- Edit text in `index.html`, then commit and push.
- Change the "Last updated" line in the footer.
- Colors live at the top of `style.css` (`:root` for light, the `prefers-color-scheme: dark` block for dark).
