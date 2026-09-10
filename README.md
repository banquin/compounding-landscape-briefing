# The Compounding Pharmacy Landscape — A Field Briefing

**v2 · reviewed 9 September 2026.** See [What's new in this edition](#whats-new-in-this-edition-september-2026) below.

A single-page, self-contained educational website explaining the **pharmaceutical compounding industry**: the value chain end to end, market size and growth, the key companies and their relative sizes, the 503A/503B regulatory split, and demand dynamics (the GLP-1 wave and what comes next). It includes a position read on **PCCA** and its software arm, **PK**, plus a 65-question self-test quiz.

It's a general-knowledge briefing built from public sources — no proprietary or confidential information.

## What's inside

- **`index.html`** — the entire site. HTML, CSS, and JavaScript are inlined into one file, so there is **no build step and no dependencies**. Open it and it works.
- Infographics (SVG/CSS): value-chain flow, an ownership map of the Precision Health Holdings family (PHH → PCCA → PK Software), market-growth chart, supplier size comparison, a software positioning quadrant, a 503A-vs-503B comparison, and a demand timeline.
- A "What changed" strip at the top summarizing, with dates, everything that moved between the first edition and September 2026, plus a regulatory-watch list in the 503A/503B section.
- A quiz engine with a 65-question bank across eight topics (Value Chain, Regulation, Market, PCCA, Players, Demand, What's New · 2026, Hard · Inference). Questions and answer order shuffle each run.

## What's new in this edition (September 2026)

Researched from public sources on 9 September 2026 and woven into every section:

- **GLP-1 compounding has effectively closed.** FDA proposed (Apr 30, 2026) excluding semaglutide, tirzepatide and liraglutide from the 503B bulks list; the Fifth Circuit upheld FDA's shortage-resolution decisions (Aug 27, 2026); waves of FDA warning letters hit telehealth marketers (Mar and Jun 2026); FDA said it would restrict GLP-1 *ingredients* headed for unapproved compounding.
- **Brands undercut compounders.** TrumpRx cash prices (Wegovy pill $149, injectables ~$350), plus two approved oral GLP-1s (Wegovy pill, Dec 2025; Foundayo/orforglipron, Apr 2026). Novo's CEO put compounded GLP-1 users at up to 1.5 million (Jan 2026).
- **Telehealth pivoted to branded.** Hims' $49 compounded pill lasted two days (Feb 2026) before an FDA statement and HHS→DOJ referral; the Mar 9 Novo–Hims deal, Ro's exit, and LifeMD's brand-only stance followed. Hims Q2 2026: $753M revenue, gross margin 64% vs 76%.
- **Peptides are the next frontier.** FDA removed 12 peptides from Category 2 (Apr 22, 2026); its advisory committee backed six of seven for the 503A bulks list (Jul 23–24, 2026) — non-binding, rulemaking pending.
- **PCCA reorganized.** Gus Bassani, PharmD, became U.S. CEO (Apr 2025); PCCA now sits under Precision Health Holdings with Eagle Analytical, the Wilcrest Pharma 503B facility and consumer incubator Curive; new ExoBlue base (May 2026), TJM Labs AI-automation partnership (Jun 2026), Compounding PATH for Technicians (Nov 2025). Long-time CEO L. David Sparks died May 9, 2026. Member count updated to 3,000+ (as reported Nov 2025).
- **Competitors.** Fagron FY2025 revenue €952M (+9.2%); H1 2026 +16% reported but +3.1% organic on U.S. GLP-1 normalization. Medisca: dsm-firmenich vitamin-API partnership (May 2026), founder Antonio Dos Santos as CEO (Jun 2026). RedSail acquired PrimeRx (Feb 2026; ~16,000 pharmacies).
- **Market data.** 2026 estimates of $6–7.5B (6–7% CAGR); APC 2025–26 Snapshot (~7,500 pharmacies, 30–40M compounded Rx/yr, HRT 36% of therapies). FDA removed boxed warnings from menopausal hormone therapy (Nov 2025).

## View it locally

Just open the file in a browser:

```bash
open index.html        # macOS
# or: xdg-open index.html   (Linux) / start index.html (Windows)
```

Or serve it (nicer for fonts/caching):

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publish it on GitHub Pages

1. Push this repo to GitHub (see below).
2. In the repo: **Settings → Pages → Build and deployment → Source: "Deploy from a branch"**, branch `main`, folder `/ (root)`.
3. Your site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Push to GitHub

This folder is already a git repository with an initial commit. To put it on GitHub:

**Option A — GitHub CLI (one command):**

```bash
gh repo create compounding-landscape-briefing --public --source=. --remote=origin --push
```

**Option B — manual:** create an empty repo on github.com (no README), then:

```bash
git remote add origin https://github.com/<your-username>/compounding-landscape-briefing.git
git branch -M main
git push -u origin main
```

## Sources & caveats

Synthesized from public market-research summaries, FDA notices, court rulings, trade press, and company materials; the full source list is in the page footer. Items marked "pending" (FDA's final 503B bulks decision, peptide rulemaking) were unresolved as of 9 September 2026. Market sizes and growth rates are third-party estimates that vary by source and definition; private-company revenues (PCCA, Medisca) and internal business-line splits are not publicly disclosed and are presented qualitatively. Figures are directional, not precise. Nothing here is investment, legal, or career advice.

## License

MIT — see `LICENSE`.
