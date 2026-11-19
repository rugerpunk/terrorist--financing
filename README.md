# ChainLogic::TF — Terrorist Financing in Crypto, Forensic Intelligence Guide

## What is ChainLogic::TF?

ChainLogic::TF is a free, interactive dashboard that teaches how **terrorist financing (TF)** and **sanctions evasion** move through virtual assets, and how a forensic investigator detects, traces and reports them.

Think of it as a hands-on field guide: instead of reading a 40-page report, you click through animated money-flow diagrams, red-flag categories, case studies and an investigation methodology built around the **FATF Virtual Assets Red Flag Indicators (September 2020)**.

The dashboard was built as teaching material for a **hands-on forensic investigation workshop funded by a Solana Foundation grant**.

## Why Was This Dashboard Built?

Future legal professionals (prosecutors, judges, compliance officers and regulators) graduate without any practical understanding of how blockchain ecosystems are weaponized for terrorism financing and international sanctions evasion.

This creates a critical enforcement gap. Courts and regulators are confronted with on-chain evidence they cannot evaluate. Meanwhile, bad actors operate with near-impunity in jurisdictions where legal expertise hasn't caught up with Web3 realities.

A concrete, urgent example is the **A7A5** ruble-backed token, documented as a mechanism for Russia to bypass OFAC sanctions through a crypto-energy transfer network involving Kyrgyz, Chinese and Hong Kong nodes.

Without accessible, practitioner-grade educational infrastructure on Solana's forensic landscape, the next generation of law professionals will remain blind to these schemes. It is imperative for us, experts in our field, to share our expertise in the best way possible, and hands-on workshops are the best way to impact the community. This dashboard is the material behind that workshop, released openly so anyone can teach with it.

## How Simple Is It?

This project is intentionally basic and straightforward:

- No frameworks like React or Vue.js. Just **one `index.html` file**: HTML, CSS and vanilla JavaScript
- Works in any modern web browser, on desktop and mobile
- No installation, no build step, no backend
- No API key required

Perfect for trainers, students, investigators and compliance teams who want to open it and start teaching or learning right away.

## What You Get

| Section | What it shows |
|---|---|
| **Workshop** | The problem statement behind the Solana Foundation grant workshop and who it's for |
| **Overview & Definitions** | TF, virtual assets, VASPs and STR/SAR explained, plus a prevalence chart and an investigator's priority matrix |
| **Why It Matters** | Six reasons virtual assets attract terrorist financing (speed, pseudonymity, micro-donations, regulatory arbitrage, darknet procurement, foreign terrorist fighter funding) |
| **TF Attack Flow Visualization** | Animated 3-phase flow (Fundraising → Layering → Deployment). Click any node to reveal forensic investigation tips |
| **Red Flag Indicators** | 36 indicators across the 6 FATF categories: Transactions, Patterns, Anonymity, Senders/Recipients, Source of Funds, Geographical |
| **Investigation Methodology** | A 5-phase framework: intelligence collection, on-chain tracing, entity attribution, international cooperation/MLA, enforcement and reporting |
| **Case Studies** | Three FATF-reported cases reconstructed through a TF forensic lens (mule networks, AlphaBay, pensioner-targeting scams) |
| **Tools & Techniques** | Blockchain analytics, OSINT and dark web, legal and reporting channels, and wallet-clustering techniques |

It also includes a **GDPR-compliant cookie banner and policy** (consent-first Google Analytics, optional preference cookies, full policy in a modal).

## Quick Setup (2 Minutes)

### Option 1: Just open it
1. Download `index.html` from this repository
2. Double-click it to open it in your browser

That's it. Everything works offline except the fonts and libraries loaded from CDNs.

### Option 2: Host it on your website
1. Upload `index.html` to any web hosting provider (or enable **GitHub Pages** on this repository)
2. Open your site's URL

### Optional: Enable Google Analytics
Analytics is **off by default**. To turn it on:

1. Open `index.html` in any text editor
2. Find the line: `window.CS_GA_ID = 'G-XXXXXXXXXX';`
3. Replace `G-XXXXXXXXXX` with your own GA4 Measurement ID
4. Save and upload

Google Analytics only loads **after** a visitor clicks *Accept* in the cookie banner.

### Optional: Adapt the cookie policy
The cookie policy names **Crypto Sentinel (gabidumitriu.ro)** as the data controller. If you host your own copy, edit the *"Who we are"* paragraph in the cookie modal so it names you instead.

## How to Use It in a Workshop

1. Start at **Workshop** to set the context: the enforcement gap
2. Walk through **Overview** and **Why It Matters** to build vocabulary
3. Use the **Flow Visualization** live: switch phases and click nodes to discuss what an investigator sees at each hop
4. Split participants into groups and assign each a **Red Flag** category
5. Analyze the **Case Studies** together, then map them to the **Methodology** phases
6. Close with **Tools & Techniques** and discuss what's available to whom (FIU, LEA, VASP, court)

## Technical Details

- **Stack:** HTML5, CSS3, vanilla JavaScript, Bootstrap 5.3.2
- **Libraries (via CDN):** Bootstrap, Bootstrap Icons, Font Awesome 6.5, Google Fonts (DM Sans, Space Mono)
- **Cookies used:**
  - `cs_consent`: strictly necessary, stores your cookie choice (180 days)
  - `cs_prefs`: preferences, only with consent, remembers the open flow phase, red-flag category and tools tab (180 days)
  - `_ga`, `_ga_<ID>`: Google Analytics, only with consent and only if a Measurement ID is configured
- **Fallback:** if the browser blocks cookies (for example, when opened as a local file), the choice is stored in `localStorage` instead

## Data Sources

- FATF (2020) — *Virtual Assets Red Flag Indicators of Money Laundering and Terrorist Financing*
- FATF Recommendation 15 and its Interpretive Note
- FATF *Guidance for a Risk-Based Approach to Virtual Assets and VASPs* (2019)
- UN Security Council Resolutions 1267 and 1373
- OFAC SDN List and EU Sanctions Map

## Limitations

- **Educational material, not legal advice.** Always verify against official FATF, OFAC, EU and UN publications before acting.
- Case studies are **reconstructed from FATF-reported cases**. They illustrate patterns and are not open investigations.
- Prevalence figures are indicative and derived from FATF case-study analysis (2017–2020).
- The dashboard does not query any blockchain. For live Solana wallet screening, see **[SolTrace](https://github.com/rugerpunk/SolTrace)**.

## Troubleshooting

**Icons or fonts not showing?**
- You're probably offline. The libraries and fonts load from CDNs and need an internet connection.

**Cookie banner keeps appearing?**
- Your browser may be blocking both cookies and local storage (for example, strict private mode). The choice is then kept only for the current visit.

**Analytics not recording anything?**
- Check that you replaced `G-XXXXXXXXXX` with a real Measurement ID and that you clicked *Accept* in the cookie banner.

## Privacy & Security

- No backend, no database, no accounts
- No personal data is collected unless a visitor explicitly consents to Analytics
- No advertising, remarketing or social-media cookies
- Consent can be changed or withdrawn at any time from the cookie button in the bottom-left corner

## Disclaimer

This dashboard is independent analytical commentary based on public FATF material. It is not affiliated with or endorsed by FATF/OECD, OFAC or the Solana Foundation, and it does not reproduce FATF materials.

## Contributing

This is an open-source project funded by a grant powered by the Solana Foundation: https://earn.superteam.fun/grants/solana-foundation-romania-grants/references/

If you find bugs, spot an outdated reference or want to add new typologies, red flags or case studies, please open an issue or a pull request. Your input helps strengthen this material for the entire community.

📌 You can find me here: [gabidumitriu.ro](https://gabidumitriu.ro)

## License

This is an open source project under the A Creative Commons (CC) license, meaning it requires Attribution (BY)—giving credit to the creator—and may combine up to three additional conditions: • BY (Attribution): Credit the creator, link to the license, and note any changes made. • SA (ShareAlike): Share any adapted or remixed work under the same (or compatible) license. • NC (NonCommercial): Allow noncommercial use only (no primary monetary compensation or commercial advantage). • ND (NoDerivatives): Share the work only in its original, unadapted form. However, please ensure proper attribution by including a reference to this repository and acknowledging the original contributor and the Solana Foundation. I deeply appreciate recognition for any future work put into building and maintaining this material.

Built with ❤️ for the Solana community
Funded by a Solana Foundation Grant
