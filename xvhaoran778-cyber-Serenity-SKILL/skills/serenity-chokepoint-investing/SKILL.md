---
name: serenity-chokepoint-investing
description: Cross-market supply-chain chokepoint investing research workflow inspired by Serenity's public posts and trade disclosures. Use when analyzing A-share, US, Hong Kong, Taiwan, Japan, Europe, or other listed stocks, sectors, or trade ideas through hidden bottlenecks, AI/semiconductor/energy infrastructure supply chains, CPO/photonics, substrates, power semis, transformers, government-backed critical supply chains, company news/announcements, or when the user asks to "use Serenity's method", "蒸馏 Serenity", "瓶颈点投资", "产业链卡点", "chokepoint investing", or to extract/organize Serenity-like trade records.
---

# Serenity Chokepoint Investing

## Core Stance

Use this skill to produce research, not financial advice. Treat Serenity's public record as a pattern library: supply-chain mapping, bottleneck detection, Bayesian evidence updating, asymmetric mispricing, and explicit evidence tracking. Do not imitate identity, certainty, returns, or promotional tone.

Always browse or otherwise verify current market facts when prices, filings, laws, customers, supply relationships, or recent catalysts matter. For live analysis, fetch company news and official announcements unless the user explicitly asks for a historical/theoretical framework only. Label inference, rumor, and unverified trade disclosure clearly.

## Workflow

1. **Identify the listing market.** Normalize ticker, exchange, reporting currency, filing regime, trading liquidity, and information sources before analysis.
2. **Fetch current news and official disclosures.** Gather recent announcements, filings, earnings, customer/supplier news, subsidies, index/listing events, dilution/financing, and credible negative reports. Use `references/market-data-and-news.md` for source priority by market.
3. **Define the end-demand shock.** Name the large demand wave: AI clusters, CPO, 800VDC, data-center power, photonics, memory, sovereign supply chains, robotics, or another concrete buildout.
4. **Map the physical chain backward.** Trace from buyer/system to module, component, material, equipment, foundry, substrate, chemical, or capacity owner. Prefer BOMs, filings, presentations, standards docs, patents, customer qualification language, and government supply-chain documents.
5. **Set the prior.** State the initial probability that this company is a true bottleneck. Anchor the prior in physical reality: BOM role, customer need, capacity, substitutes, and company scale.
6. **Dig down at least three layers.** Do not stop at the obvious bottleneck. Move from GPU/HBM/power/network into second- and third-order nodes: laser sources, substrates, crystal growth equipment, testing, packaging, fiber, chemicals, tools, and overlooked system integrators.
7. **Find the chokepoint.** Identify where supply is scarce, slow to expand, architecturally specific, or concentrated. Look for quasi-monopoly share, proprietary process, qualification cycles, national-security status, or upstream material dependence.
8. **Translate demand into financial impact.** Ask whether the same demand shock is immaterial to mega-caps but material to this smaller company. Estimate revenue, margin, backlog, or multiple impact.
9. **Test market access and pricing vacuum.** Check market cap, analyst coverage, liquidity, float, short interest, institutional ownership constraints, index/listing events, and whether large funds are structurally unable to own the name before the rerating.
10. **Test mispricing.** Compare the chokepoint's future relevance with current market attention, market cap, book value/replacement value, forward earnings scenarios, balance sheet risk, liquidity, dilution, and ownership structure.
11. **Update with evidence.** Treat new filings, earnings, customer wins, subsidies, technical validation, short reports, dilution, and failed ramps as Bayesian evidence that raises or lowers conviction.
12. **Track capital rotation.** Identify whether institutions are rotating from first-order winners into second-order suppliers, for example memory -> optical modules -> external light sources / silicon photonics.
13. **Score the setup.** Use the rubric in `references/research-rubric.md` when the user asks for a formal analysis or when multiple candidates are compared.
14. **Separate trade from thesis.** Record only explicit trade disclosures as trades. Treat "bullish", "favorite", "compelling", price targets, and sector lists as thesis or watchlist unless the source says bought/went long/took positions/adding/sold/trimmed/own/hold.
15. **Write the output with evidence levels.** Include strongest evidence, weakest link, near-term catalysts, disconfirming evidence, and what would change the thesis.

## Output Shape

For a single company, produce:

- **Verdict:** one-line thesis and confidence level.
- **Market Context:** listing venue, currency, liquidity, disclosure source quality, and latest news/announcement window checked.
- **Chokepoint:** exact supply-chain node and why it matters.
- **Evidence:** sourced facts, then inferences.
- **Bayesian Update:** prior, positive evidence, negative evidence, posterior direction.
- **Mispricing:** market-cap/valuation mismatch, timing, and why the market may miss it.
- **Market Microstructure:** float/liquidity, short interest, analyst coverage, institutional ownership constraints, and possible reflexive effects.
- **Risks:** substitution, customer concentration, capacity expansion by rivals, dilution, cyclicality, liquidity, regulatory/geopolitical issues.
- **Catalysts:** filings, earnings calls, customer ramps, standards transitions, subsidies, index/listing events.
- **Trade Disclosure Handling:** whether there is an explicit trade disclosure, a thesis-only mention, or no usable disclosure.
- **Open Checks:** facts that need fresh verification.

For a basket or sector, produce a table with: `Candidate | Supply-chain node | Chokepoint strength | Evidence quality | Mispricing signal | Catalyst | Key risk | Confidence`.

## Serenity-Specific Heuristics

- Favor non-obvious upstream suppliers over obvious end winners.
- Favor small companies where a real-world demand shock can change financials, not just headlines.
- Require a "why this company, not the obvious giant?" answer.
- Prefer architecture-dependent nodes: lasers, substrates, epiwafers, FAU, CPO packaging, optical engines, power semis, switchgear, transformers, specialized foundries, high-purity chemicals.
- Treat "government named this as critical" as evidence, not a complete thesis.
- Treat low P/B or replacement value as useful only when the asset is tied to a future growth bottleneck.
- Look for customer pull: hyperscaler, Nvidia/AMD/Broadcom/Marvell, cloud, Apple, SpaceX, government, or top foundry qualification.
- Convert product adoption into company-level impact: revenue growth, gross margin, backlog, forward P/E, sales multiple, or replacement value.
- Treat company news as an evidence stream: announcements and filings update conviction; media headlines merely point to facts that need verification.
- Treat short squeeze, low float, and retail attention as accelerants, not the core thesis.
- Penalize analyses that stop at first-order bottlenecks already crowded by institutions.
- Penalize stories that rely only on vibes, social momentum, or historical returns.

## Resources

- Read `references/research-rubric.md` for the scoring matrix, trade-disclosure labels, and reusable output templates.
- Read `references/market-data-and-news.md` when analyzing a live company, especially across A-shares, US stocks, Hong Kong stocks, or other markets with different disclosure systems.
- Read `references/pattern-library.md` when the user asks to generate ideas, screen candidates, or explain Serenity's reusable pattern from examples.
