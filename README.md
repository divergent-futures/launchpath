# Launchpath — Launch Smarter, Keep What You Build

**A free, private, open toolkit that tells first-time creators the truth about crowdfunding** — their real odds, the moves that actually change them, and real campaigns like theirs — built from **590,000 real Kickstarter projects**.

**▶ Use it: [divergentfutures.co/launchpath](https://divergentfutures.co/launchpath/)** · **[Download it](https://divergentfutures.co/launchpath/launchpath.html)** *(one file, works offline, forever)*

A [Divergent Futures](https://divergentfutures.co) project. Working title — name may change.

---

## What it does

1. **Learn your real odds.** Not "Technology: hard." Your actual subcategory: DIY electronics funds at ~52%, apps at ~7%. Plus how big and crowded your corner is, so you know before committing a year to the wrong shape.
2. **Score your readiness.** Eleven plain questions against the factors that move funding. Five of them — goal size, preparation time, campaign duration, video, pre-launch audience — carry weights **fitted against 57,982 recent campaigns** (2023+, subcategory-controlled). The other six — prototype, manufacturing costing, delivery padding, risks honesty, reward simplicity, idea-testing — are judgement, and the tool labels which is which instead of passing opinion off as measurement. No sugarcoating: if you're not ready yet, it'll say so — and if you are, it'll say that too.
3. **See real campaigns like yours.** A full written report compares you to the field and shows real matched campaigns — funded, near-miss, and failed — each linked to its real Kickstarter page.
4. **Fix the gaps, then launch** — owning 100% of what you made. Every weak answer comes back as a ranked fix list: what to change, in what order, and how many points each fix is worth.

## The privacy model (the whole point)

**Nothing you type ever leaves your device.** This is a single static HTML file: no server, no accounts, no analytics, no cookies, no storage, zero network requests. Your idea and your answers exist only in your browser tab.

Don't trust us — verify: open your browser's dev tools, watch the Network tab, use the tool. Nothing is transmitted. The entire source is this repository.

Why so strict? Because the target users are young creators typing their one good idea — often pre-patent — into a web page. The only privacy policy that means anything is being *structurally incapable* of collecting anything.

## The data & method (honest version)

- **Baseline:** 378,662 Kickstarter projects (2009–2017, the public research dataset) — used for absolute success-rate benchmarks (category/subcategory rates, the goal-size gradient).
- **Current snapshot:** 210,806 projects (public Web Robots crawl through June 2026) — used for current volumes, subcategory sizes/shares, and the example database. *Known bias, handled:* monthly crawls over-sample successful projects, so we never quote recent absolute rates — only rankings, shares, and volumes, where the bias can't mislead.
- **The 5,000-campaign example database:** a stratified sample — 2,500 funded across the winning range, 1,500 near-misses (50–99%; deliberately over-sampled because they teach the most), 1,000 clear failures — across all 15 categories and 160 subcategories, 84% launched 2024–2026, extra density in Technology/Design/Games. Quality rules: Kickstarter's own `percent_funded` figure used verbatim; canceled campaigns ≥50% excluded (a creator pulling the plug isn't a market verdict); every record links to its live public page.
- **Scoring weights:** the five measurable factors are fitted by logistic regression with subcategory fixed effects on 57,982 campaigns launched 2023+ (89 subcategories, n≥150 each). The six judgement factors keep weights grounded in published research and platform rules — Kickstarter's creator rules (working-prototype requirement, Risks & Challenges), Mollick's *Delivery Rates on Kickstarter* (SSRN), UCLA DataRes' 378k-campaign analysis, DTU Science Park hardware post-mortems — and are labelled `judgement` in the report so you always know which kind of claim you're reading.
- **Estimates are estimates.** The odds figure guides decisions; it doesn't promise outcomes, and the tool says so wherever it appears.

## Who it's for

Student makers and first-time hardware creators — and the clubs, school programs, and youth-entrepreneur communities that support them. It runs anywhere a browser runs, needs no accounts or setup, and is free.

## Independence

Not affiliated with, or endorsed by, Kickstarter. All statistics derive from publicly available data; all examples are real public campaigns, linked to their pages.

## Contributing / feedback

Issues and PRs welcome — especially from people who have actually run campaigns. If a number looks wrong, say so; the receipts-not-hype rule means we'd rather fix it than defend it.

## License

MIT — see [LICENSE](LICENSE). Campaign facts referenced are public data; campaign names and pages remain their creators' own.
