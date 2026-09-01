# Launchpath — Launch Smarter, Keep What You Build

**A free, private, open toolkit that tells first-time creators the truth about crowdfunding** — their real odds, the moves that actually change them, and real campaigns like theirs — built from **590,000 real Kickstarter projects**.

**▶ Use it: [divergentfutures.co/launchpath](https://divergentfutures.co/launchpath/)**

A [Divergent Futures](https://divergentfutures.co) project — [more about Launchpath](https://divergentfutures.co/projects/launchpath/).

---

## What it does

1. **Learn your real odds.** Not "Technology: hard." Your actual subcategory: DIY electronics funds at ~52%, apps at ~7%. Plus how big and crowded your corner is, so you know before committing a year to the wrong shape.
2. **Score your readiness.** Eleven plain questions across the eleven factors that separate prepared campaigns from unprepared ones — goal size, preparation time, campaign duration, pre-launch audience, working prototype, real manufacturing costing, demo video, idea-testing, delivery-date realism, reward structure, and an honest risks section. You get a score out of 100, a verdict band, and a ranked list of what to fix first.
3. **See real campaigns like yours.** A full written report compares you to the field and shows real matched campaigns — one that made it, one that came heartbreakingly close, one that didn't — each linked to its real Kickstarter page. Every weak factor also opens onto a matched pair: a campaign that did that specific thing well, next to one that didn't.
4. **Fix the gaps, then launch** — owning 100% of what you made.

## The privacy model (the whole point)

**Nothing you type ever leaves your device.** This is a single static HTML file: no server, no accounts, no analytics, no cookies, no storage, zero network requests. Your idea and your answers exist only in your browser tab.

Don't trust us — verify: open your browser's dev tools, watch the Network tab, use the tool. Nothing is transmitted. The entire source is this repository.

Why so strict? Because the target users are young creators typing their one good idea — often pre-patent — into a web page. The only privacy policy that means anything is being *structurally incapable* of collecting anything.

## The data & method (honest version)

- **Current headline rates (Kickstarter's audited Annual Benefit Statements):** **58.2%** of projects funded platform-wide in 2025, and **34%** for first-time creators, who launched 66% of everything that year (39% in both 2023 and 2024). These are the current figures and the ones the tool leads with. The 2009–2017 dataset understates the platform today by roughly eighteen points, so it is never quoted as a current rate.
- **Baseline:** 378,662 Kickstarter projects (2009–2017, the public research dataset) — **the 2009–2017 dataset**, and the source used for *relative* absolute benchmarks: how rates differ between categories, subcategories and goal sizes. It is not a current rate. (It was previously described here as a "complete census"; the public Kaggle set is a Web Robots extract holding 378,661 — one off — and the census claim is unverified, so the wording was corrected on 2026-08-28.)
- **Current snapshot:** 210,806 projects (public Web Robots crawl through June 2026) — used for current volumes, subcategory sizes/shares, and the example database. *Known bias, handled:* monthly crawls over-sample successful projects, so we never quote recent absolute rates — only rankings, shares, and volumes, where the bias can't mislead.
- **The absolute-versus-relative rule** is the single most important methodological commitment in this project. Any absolute rate you see comes from the 2009–2017 dataset and is labelled with that period. Anything derived from the 2026 crawl is expressed as a comparison. The two are never mixed, and the combined "590,000" figure describes scale — it is never the denominator of a quoted rate.
- **The 5,000-campaign example database:** a stratified sample — 2,500 funded across the winning range, 1,500 near-misses (50–99%; deliberately over-sampled because they teach the most), 1,000 clear failures — across all 15 categories and 160 subcategories, 84% launched 2024–2026, extra density in Technology/Design/Games. Quality rules: Kickstarter's own `percent_funded` figure used verbatim; canceled campaigns ≥50% excluded (a creator pulling the plug isn't a market verdict); every record links to its live public page.

## How sure we are of the score, factor by factor

This is the part most tools hide, so it gets its own section.

- **Five of the eleven factors are `measured`** — their weights are fitted on **57,982 campaigns from 2023 onward** (a filtered subset of the current snapshot, 89 subcategories, with subcategory fixed effects).
- **The other six are `judgement`.** They describe things that do not exist as fields in any public dataset and never will — whether a prototype actually works, whether the manufacturing was really costed. Those weights are reasoned, argued for, and open to challenge. They are not fitted, and we don't pretend otherwise.
- **Every row of the score breakdown is labelled `measured` or `judgement`**, so the split is visible at a glance instead of hidden behind one confident number. Overall the split is **52 of the 100 points measured, 48 judgement**.
- The judgement weights draw on Kickstarter's own video statistics (54% funded with video vs 39% without) and creator rules (working-prototype requirement, Risks & Challenges), Mollick's *Delivery Rates on Kickstarter* (SSRN), UCLA DataRes' 378k-campaign analysis, DTU Science Park hardware post-mortems, and large-scale campaign studies.
- **The conversion from log-odds into points is a ranking, not a precise measurement**, and the 85 / 70 / 45 verdict cut-offs are communication devices rather than findings.
- **Known modelling choice, stated plainly:** goal size counts twice — once inside the readiness score, and again as the base rate the odds are built from. There is a written defence for this. It has not yet been externally attacked, so don't treat it as settled.

## What it isn't

- **Not a predictor.** The odds figure is a historical base rate adjusted for two things we can observe — what you're asking for, and what you're asking it in. It tells you what happened to campaigns that looked like yours. It does not tell you what will happen to yours.
- **Not a gatekeeper.** It will never tell you not to launch. That call is yours; the tool's job is to make sure you make it with the real numbers in front of you.
- **Not validated by real users yet.** The model has been through adversarial review, but no first-time creator has yet used this in a recorded think-aloud. Treat it as carefully built, not as proven.
- **Not affiliated with Kickstarter**, and not a business. Nothing is sold, upsold, or gated.

## Who it's for

Student makers and first-time hardware creators — and the clubs, school programs, and youth-entrepreneur communities that support them. It runs anywhere a browser runs, needs no accounts or setup, and is free.

Note for creators under 18: Kickstarter requires project creators to be 18 or over. Minors can work on a project, but the account needs an adult creator with government-issued ID and a bank account in their name — or a fiscal sponsor holding the legal entity on the team's behalf. The tool says this up front rather than burying it.

## Independence

Not affiliated with, or endorsed by, Kickstarter. All statistics derive from publicly available data; all examples are real public campaigns, linked to their pages.

## Contributing / feedback

Issues and PRs welcome — especially from people who have actually run campaigns. If a number looks wrong, say so; the receipts-not-hype rule means we'd rather fix it than defend it.

Contact: [space.divergentfutures@gmail.com](mailto:space.divergentfutures@gmail.com)

## License

MIT — see [LICENSE](LICENSE). Campaign facts referenced are public data; campaign names and pages remain their creators' own.
