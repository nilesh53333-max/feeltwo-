# FeelTwo Favicon Pack

## Files included

| File | Size | Purpose |
|------|------|---------|
| `favicon.ico` | 16+32+48 (multi-res) | Universal — every browser, including IE |
| `favicon.svg` | scalable | Modern browsers (Chrome, Firefox, Safari) — sharp at any zoom |
| `favicon-16x16.png` | 16×16 | Browser tab |
| `favicon-32x32.png` | 32×32 | Browser tab (high-DPI) |
| `favicon-48x48.png` | 48×48 | Windows site shortcut |
| `favicon-96x96.png` | 96×96 | Google TV |
| `favicon-192x192.png` | 192×192 | Android home screen |
| `favicon-512x512.png` | 512×512 | PWA / app icon |
| `apple-touch-icon.png` | 180×180 | iOS home screen bookmarks |

## Installation

### Step 1 — Upload all files to your repo's root folder

In your `feeltwo.com` GitHub Pages repo, drop every file from this pack into the **same folder as `index.html`** (the root). They should sit alongside your existing files, not inside any sub-folder.

### Step 2 — Add these `<link>` tags to `<head>` in `index.html`

Paste this block inside `<head>`, ideally near the top, after `<meta charset>` and `<title>`:

```html
<!-- Favicons -->
<link rel="icon" type="image/svg+xml" href="/favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="shortcut icon" href="/favicon.ico">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="192x192" href="/favicon-192x192.png">
<meta name="theme-color" content="#25D366">
```

### Step 3 — Commit and push

```bash
git add favicon* apple-touch-icon.png
git commit -m "add favicon pack"
git push
```

GitHub Pages takes 1–5 minutes to deploy.

### Step 4 — See the change

**Important:** browsers cache favicons HARD. To see the new icon immediately:

- Open in **incognito / private window** — best way to verify it works
- Or do a **hard refresh**: Ctrl+Shift+R (Windows) / Cmd+Shift+R (Mac)
- Or close and reopen the tab

If the globe is still showing after 24h in incognito, check the deploy worked by going to `https://feeltwo.com/favicon.ico` directly — you should see the icon.

## What it looks like

The favicon is a simplified version of the FeelTwo logo: just the house silhouette + WhatsApp chat bubble tail in WhatsApp green (`#25D366`), with a white door negative space. The interior windows are dropped at small sizes because they blur into noise below 64px.

## Bonus: theme-color

The `<meta name="theme-color" content="#25D366">` tag tints the browser address bar on Android Chrome to match your brand. Worth keeping.
