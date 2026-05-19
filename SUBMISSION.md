# FADE — Submission Pack

Public artifacts for grant/incentive/listing submissions.

---

## Quick links (copy-paste ready)

| Field | Value |
|---|---|
| Project name | **FADE** |
| Tagline | long the truth. fade the cope. |
| Category | Prediction Markets / DeFi / Consumer Crypto |
| Repository | https://github.com/santuy69/fade-landing |
| Live demo | https://santuy69.github.io/fade-landing/ |
| License | MIT |
| Stage | Concept landing / pre-launch |
| Chain | Base (settlement in USDC) |
| Contact | @0x_Missy22 (X) |

---

## Project descriptions (pick by length)

### One-liner (60 chars)
> Onchain prediction markets for crypto-native traders.

### Tweet (280 chars)
> FADE — onchain prediction markets settled in USDC on Base. Bet on
> elections, BTC/ETH price targets, AI shipping deadlines, sports,
> geopolitics. Self-custody, sub-cent gas, no KYC, no admin queue.
> Long the truth. Fade the cope.

### Short (≤ 100 words)
> FADE is an onchain prediction market built for crypto-native traders.
> Every market resolves to YES or NO between 1¢ and 99¢ — that price is
> the live, capital-weighted probability of the outcome. Users connect
> any EVM wallet, deposit USDC on Base, take positions, and exit anytime.
> When markets resolve, winning shares pay $1.00 automatically — no
> admin, no withdrawal queue, no permission. We focus on the topics
> Polymarket undersells: AI shipping deadlines, memecoin flips, on-chain
> KPIs, and crypto-native politics.

### Medium (≤ 250 words)
> **FADE** is a prediction-market protocol designed for crypto-native
> users who already trade narratives on X — but currently have no way to
> price them in capital. Every market is a binary YES/NO contract priced
> 1¢–99¢ in USDC; the price is the market-implied probability and updates
> live as orders cross.
>
> The protocol settles on **Base** for sub-cent gas and CEX-like UX, with
> self-custody throughout. There is no KYC, no admin-controlled
> withdrawal queue, and no centralized market-resolution ticket system —
> resolution is verified onchain via oracle commits, and winning shares
> auto-pay $1.00 each on resolve.
>
> **What FADE focuses on that others miss:** AI shipping deadlines (GPT-6,
> Claude release windows, model benchmark thresholds), memecoin flips
> (PEPE/DOGE marketcap, sector rotations), on-chain KPIs (BTC dominance,
> ETF flow gates, dominance bands), and crypto-native politics (Fed Chair
> decisions, regulatory deadlines). These markets historically have the
> highest velocity on Polymarket but are buried under generic election
> contracts.
>
> **Stage.** This repository is the public landing concept page —
> production contracts and orderbook are in private development. The
> landing is intentionally degen-coded: acid-lime accent, neon-green YES,
> hot-pink NO, terminal mono UI. It signals to crypto-native users that
> this isn't an institutional product wearing crypto skin.
>
> MIT-licensed. Built solo. Deployed on GitHub Pages.

### Long (≤ 500 words)
> **FADE** is an onchain prediction-market protocol built specifically for
> crypto-native traders. Every market is a binary YES/NO contract priced
> between 1¢ and 99¢ in USDC. Price equals the live, capital-weighted
> probability of the outcome — pay 62¢ for a YES share, get $1.00 if you
> win, $0.00 if you lose, exit anytime in between at the live mid.
>
> **Why now.** Twitter/X is full of degens calling outcomes — Fed cuts,
> ETH/BTC ratio breaks, model release windows, sport outcomes — but
> outside Polymarket there is no liquid, low-friction venue to convert
> conviction into capital onchain. Polymarket optimizes for institutional
> /political markets and US-policy compliance; FADE optimizes for
> crypto-native edges that Polymarket explicitly deprioritizes.
>
> **Architecture.**
> 1. **Settlement layer** — Base mainnet, USDC, sub-cent gas, EVM-native.
> 2. **Markets** — binary YES/NO via fungible position tokens; orderbook
>    + AMM hybrid for thin-liquidity markets.
> 3. **Resolution** — onchain commit-reveal oracle with multi-sig escape
>    hatch for ambiguous outcomes. No admin queue, no withdrawal lock.
> 4. **UI** — single-file PWA, no KYC wall, wallet-only login, no email,
>    no analytics ID, no mandatory cookies.
>
> **Categories at launch:**
> - 🪙 Crypto (BTC/ETH price targets, dominance, ETF approvals)
> - 🤖 AI (model release windows, benchmark thresholds)
> - 🎰 Memes (sector rotations, marketcap flips)
> - 📉 Macro (Fed actions, recession declarations)
> - 🗳️ Politik / Geopol (regulatory deadlines, election binaries)
> - ⚽ Sports (high-volume finals, championship odds)
>
> **Differentiation.**
> - **Crypto-native taxonomy.** Categories like "Pump", "Rug", "Whales"
>   reflect how the audience actually thinks. Polymarket's UX is built
>   for journalists; FADE's UX is built for the timeline.
> - **Instant payout, no admin.** Resolved markets auto-pay onchain.
> - **No KYC.** Self-custody throughout. The wallet is the account.
> - **Sub-cent gas.** Base settlement makes 5¢ trades viable.
>
> **Stage and ask.** This repo hosts the public landing page concept and
> brand identity. Smart contracts, orderbook engine, and oracle layer are
> in private development. Looking for: ecosystem support / grants / co-
> marketing with Base-aligned protocols, and integration partners on the
> oracle resolution side.
>
> **Public artifacts.**
> - Repo: https://github.com/santuy69/fade-landing
> - Live: https://santuy69.github.io/fade-landing/
> - Operator: @0x_Missy22 (X)
>
> MIT licensed. Self-funded. One operator.

---

## Tech stack

- **Frontend (this repo):** Plain HTML/CSS/JS, single self-contained file.
  Space Grotesk + JetBrains Mono. No build, no framework, no CDN
  dependencies for app logic.
- **Settlement (planned):** Base L2, USDC native, EVM-compatible
  contracts.
- **Markets (planned):** Hybrid orderbook + LMSR AMM for thin markets.
- **Resolution (planned):** Commit-reveal oracle + multisig escape hatch.
- **Wallet:** Any EVM wallet (MetaMask, Rabby, WalletConnect).

---

## Screenshots (proof bundle)

All located in `/proof` and committed to the repo. Direct GitHub raw URLs:

| File | Use case | Size |
|---|---|---|
| `proof/landing-desktop.png` | Main desktop screenshot — submit forms | 1440×1080 |
| `proof/landing-fullpage.png` | Full scroll capture — show all sections | 1200×1200 |
| `proof/landing-hero.png` | OG image / preview card / X share | 1200×630 |
| `proof/landing-mobile.png` | Mobile responsive proof | 420×315 |

Direct raw URLs (use these in submission forms that accept image links):

- https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-desktop.png
- https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-fullpage.png
- https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-hero.png
- https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-mobile.png

---

## Verification proofs

```
$ curl -sI -L https://santuy69.github.io/fade-landing/
HTTP/2 200
server: GitHub.com
content-type: text/html; charset=utf-8
last-modified: 2026-05-19T13:23:02 GMT
strict-transport-security: max-age=31556952
```

```
$ git log --oneline
af8ff2e init: FADE landing page
```

```
$ ls -lh
-rw-r--r--  index.html     30K
-rw-r--r--  README.md      1.4K
-rw-r--r--  LICENSE        1.1K
-rw-r--r--  SUBMISSION.md  this file
drwxr-xr-x  proof/         desktop/mobile/hero/fullpage PNGs
```

---

## License

MIT — see `LICENSE`.
