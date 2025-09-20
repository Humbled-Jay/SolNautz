# SolNautz Website

A single-page marketing site for the SolNautz Solana NFT project. Built from a static HTML template and customized with SolNautz branding, links, and assets.

## Features
- Navbar with logo and quick links
- Hero with frosted background image (`assets/Background/hero.jpg`)
- Ticker/keywords strip
- About + Core Values cards
- Collection gallery (lazy-loaded images)
- How to Mint cards with image buttons (LaunchMyNFT, Magic Eden, Tensor, plus static images)
- Roadmap, FAQ, and Community CTA with X, Discord, and MagicEden links
- Basic SEO/Open Graph + JSON‑LD Organization metadata

## Getting Started
1. Open this folder in your editor.
2. Start a local server (Python example):
   ```bash
   # from the project root
   python3 -m http.server 8080
   ```
3. Visit `http://localhost:8080`.

> Tip: If you don’t see recent changes, hard refresh your browser (Cmd+Shift+R on macOS).

## Project Structure
```
SolNautz - Website/
├─ index.html                 # Main page (all markup + CSS)
├─ README.md                  # This file
├─ backups/                   # Timestamped HTML + full-site ZIP backups
├─ assets/
│  ├─ Background/
│  │  └─ hero.jpg            # Hero background image
│  ├─ buttons/               # PNG buttons and static images used in Mint section
│  │  ├─ LaunchMyNft Button.png
│  │  ├─ ME Button.png
│  │  ├─ Tensor Button.png
│  │  ├─ mint.png
│  │  ├─ wallets.png
│  │  └─ wallet2.png
│  ├─ logo/
│  │  └─ logo.png            # Small brand mark used in the navbar
│  └─ nfts/                  # Collection thumbnails
│     ├─ solnautz-01.jpeg
│     ├─ solnautz-02.jpeg
│     ├─ solnautz-03.jpeg
│     └─ solnautz-04.jpeg
```

## Customization
- Brand colors: edit CSS variables near the top of `index.html` under `:root`.
- Navbar logo: replace `assets/logo/logo.png` (28×28 or higher).
- Hero background: replace `assets/Background/hero.jpg`.
- NFT gallery: add images to `assets/nfts/` (use consistent aspect ratio; square works best). Update captions/alt text in the Collection section if desired.
- Mint buttons: replace PNGs in `assets/buttons/` (filenames already wired in the HTML).
- External links to update (search inside `index.html`):
  - LaunchMyNFT: `https://launchmynft.io/sol/17481`
  - Magic Eden: `https://magiceden.us/marketplace/solnautz___`
  - Tensor: `https://www.tensor.trade/trade/solnautz_nft`
  - X/Twitter: `https://x.com/SolNautz`
  - Discord invite (CTA): `https://discord.gg/byWmMRnCDh`

## SEO/Social
- Page `<title>` and meta description live in the `<head>` of `index.html`.
- Open Graph/Twitter image currently uses a placeholder URL; swap with your hosted image if needed.
- JSON‑LD Organization schema lists SolNautz URLs (X, LaunchMyNFT, MagicEden).

## Deploy
- Any static host works: Netlify, Vercel, GitHub Pages, Cloudflare Pages, S3/CloudFront, etc.
- Upload the entire folder contents (excluding `backups/`), or connect a repo and set the output directory to the project root.

## Backups
- Manual backups are stored in `backups/` (timestamped HTML and a full ZIP). Safe to delete older backups if needed.

## License
Private project files for SolNautz.
