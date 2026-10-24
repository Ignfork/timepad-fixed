# TimePad ($TIMEPAD)

A single-file site: `index.html`. There's no build step and no folders, so you can deploy it straight to Vercel, GitHub Pages or Netlify.

## Edit before launch
Open `index.html` and find `CONFIG` at the top of the script:
- `xUrl` / `xHandle`: your X account
- `ca`: the $TIMEPAD contract address
- `buyUrl`: where the "BUY $TIMEPAD" buttons go

## What's in it
- **Explore:** a pixel post-office scene whose clock tower shows the real local time, with Night, Dawn and Day modes. Below it are live ZEC price and Zcash block height (fetched from CoinGecko and Blockchair, with a "—" if they're unreachable), the stamp wall, how it works, and an activity feed.
- **Stamp a File:** real in-browser SHA-256 hashing of any file or pasted text (nothing is uploaded). It produces a zOpenTimestamps-style `.zots` proof you can download, and a verifier that checks a proof against the original file.
- **Launch:** a 16×16 pixel editor with pencil, fill, eraser, mirror, a CLOCK button (draws the current time), shuffle and clear. You pick a name, ticker and ZEC denomination, and can choose to list it straight away.
- **Market, Portfolio and $TIMEPAD** pages.

## Before launch
Proofs are marked PENDING (preview), not anchored on-chain. Stamps you issue are saved in the browser and marked PREVIEW, and sample stamps are marked SAMPLE.
Real anchoring on Zcash and ZEC trading need a backend and Zcash wallet integration, which this static build doesn't include.
