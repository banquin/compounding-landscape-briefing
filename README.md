# The Compounding Pharmacy Landscape — A Field Briefing

A single-page, self-contained educational website explaining the **pharmaceutical compounding industry**: the value chain end to end, market size and growth, the key companies and their relative sizes, the 503A/503B regulatory split, and demand dynamics (the GLP-1 wave and what comes next). It includes a position read on **PCCA** and its software arm, **PK**, plus a 42-question self-test quiz.

It's a general-knowledge briefing built from public sources — no proprietary or confidential information.

## What's inside

- **`index.html`** — the entire site. HTML, CSS, and JavaScript are inlined into one file, so there is **no build step and no dependencies**. Open it and it works.
- Infographics (SVG/CSS): value-chain flow, market-growth chart, supplier size comparison, a software positioning quadrant, a 503A-vs-503B comparison, and a demand timeline.
- A quiz engine with a 42-question bank across six topics (Value Chain, Regulation, Market, PCCA, Players, Demand). Questions and answer order shuffle each run.

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

Synthesized from public market-research summaries, FDA notices, trade press, and company materials. Market sizes and growth rates are third-party estimates that vary by source and definition; private-company revenues (PCCA, Medisca) and internal business-line splits are not publicly disclosed and are presented qualitatively. Figures are directional, not precise. Nothing here is investment, legal, or career advice.

## License

MIT — see `LICENSE`.
