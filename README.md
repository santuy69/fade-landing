# FADE — onchain prediction markets

> long the truth. fade the cope.

A landing page for **FADE**, an onchain prediction-market concept built for crypto-native traders. Bet on elections, BTC/ETH price targets, AI shipping deadlines, sports, and geopolitics — settled in USDC on Base.

**Live demo:** https://santuy69.github.io/fade-landing/

## Stack

- Plain HTML / CSS / JS — single self-contained file
- Space Grotesk + JetBrains Mono (Google Fonts)
- No build step, no framework, no CDN dependencies for logic
- Dark UI: acid lime accent (`#bfff00`), neon green YES (`#00ff88`), hot pink NO (`#ff2d8d`)

## Sections

- Top ticker — live BTC/ETH/SOL + protocol stats
- Hero with auto-incrementing 24h volume counter
- Trust strip (Base mainnet, no KYC, self-custody, sub-cent gas)
- Featured market card with Long/Short actions
- Top degens leaderboard + 24h volume widget
- Live activity ticker (marquee)
- 8-card hot markets grid (politics, crypto, AI, memes, macro, sports)
- 3-step onboarding
- CTA strip
- Footer with degen disclaimer

## Run locally

```bash
# Just open the file in any browser
xdg-open index.html
# or
python3 -m http.server 8080
```

## Deploy

GitHub Pages is enabled from `main` branch root. Any push to `main` redeploys automatically.

## Disclaimer

Concept design. Not deployed as a real product. Not financial advice. Not a security. DYOR. NFA.

## License

MIT
