# Serenity Chokepoint Research Rubric

Use this reference when producing a formal Serenity-style analysis, comparing candidates, or extracting trade records.

## Scorecard

Score each dimension from 0 to 5. Use half points when useful.

| Dimension | 0-1 | 2-3 | 4-5 |
|---|---|---|---|
| End-demand shock | Vague theme | Clear demand wave but uncertain timing | Specific near-term buildout with strong capex/customer pull |
| Chain specificity | Generic supplier | Plausible chain node | Exact BOM/process/material/equipment node |
| Layer depth | Obvious first-order winner only | Second-order node identified | Multi-layer map with overlooked second/third-order chokepoint |
| Bottleneck strength | Many substitutes | Some concentration or qualification friction | Scarce capacity, high switching cost, long qualification, quasi-monopoly, or critical material |
| Architecture lock-in | Commodity exposure | Some design-specific exposure | Tied to a new architecture or standard that changes supplier economics |
| Evidence quality | Social claims only | Company materials plus secondary support | Filings, customer docs, government docs, earnings calls, technical docs, multiple corroborating sources |
| News/disclosure freshness | No recent disclosure check | Some recent news checked | Recent official disclosures plus news triaged into thesis-confirming/weakening/noise |
| Mispricing | Already obvious/expensive | Some undercoverage or valuation gap | Small/ignored asset with large future relevance and plausible rerating path |
| Demand-to-financial translation | Theme cannot move numbers | Plausible but rough revenue/margin impact | Concrete unit, revenue, backlog, or consensus-beat path |
| Bayesian update quality | No update criteria | Some positive/negative evidence listed | Clear prior, posterior direction, and thesis-breaking evidence |
| Financial durability | Weak balance sheet or heavy dilution | Mixed but survivable | Balance sheet, subsidy, backlog, or cash flow reduces blow-up risk |
| Catalyst path | None | Medium-term proof points | Near-term earnings, customer launch, subsidy, index/listing, standard transition, or capacity ramp |
| Downside control | Binary or fraud-like | Volatile but analyzable | Replacement value, cash, subsidies, or strategic value limits downside |
| Reflexivity/liquidity risk | Microcap mania only | High volatility but real thesis | Liquidity/ownership considered without making it the core thesis |
| Institutional rotation | No capital-flow view | Plausible sector rotation | Clear prior winners, next layer, and evidence of capital moving |

Suggested interpretation:

- `40+`: compelling chokepoint candidate; still verify current facts.
- `30-39`: worth deeper due diligence.
- `20-29`: watchlist only unless new evidence appears.
- `<20`: mostly narrative.

## Trade Disclosure Labels

Use these labels consistently:

| Label | Include as trade? | Trigger language |
|---|---:|---|
| Explicit buy/long | Yes | bought, went long, took positions, initiated, Trade Idea: Long |
| Add/increase | Yes | adding, added, scaled, personally adding to positions |
| Hold/own | Yes, as holding | I hold, I own, personally long, comfortable hold |
| Sell/reduce | Yes | sold, sold off, trimmed, cut exposure |
| No position | Yes, as non-holding disclosure | no positions, don't plan on initiating |
| Thesis-only | No | bullish, favorite, compelling, price target, high conviction, should rerate |
| Basket disclosure | Yes, low/medium confidence | own most/not all; positions across theme |
| Retrospective disclosure | Yes, mark timing uncertain | went long last year, when I took positions, from when I went long |

## Research Template

```markdown
# [Company/Ticker] Chokepoint Analysis

## Verdict
[One-sentence thesis, confidence, and whether it is tradeable now or only a watchlist item.]

## Market Context
- Listing venue:
- Currency:
- Latest filing period checked:
- News/announcement window checked:

## Demand Shock
- End market:
- Timing:
- Why now:

## Supply-Chain Map
Buyer/system -> module -> component -> material/equipment/foundry -> company node

## Chokepoint
- Scarcity:
- Switching/qualification friction:
- Architecture specificity:
- Capacity expansion constraints:

## Evidence
| Claim | Evidence | Source | Strength |
|---|---|---|---|

## News and Disclosure Update
| Date | Source | Item | Thesis impact | Evidence strength | Follow-up |
|---|---|---|---|---|---|

## Bayesian Update
- Prior:
- Positive evidence:
- Negative evidence:
- Posterior direction:
- Thesis-breaking evidence:

## Mispricing
- Current market framing:
- Alternative framing:
- Valuation signal:
- Scenario math:

## Market Microstructure
- Analyst coverage:
- Float/liquidity:
- Short interest:
- Institutional ownership constraints:
- Reflexivity risk:

## Catalysts
- Near-term:
- Medium-term:

## Risks and Disconfirmers
- Technical substitution:
- Customer/supplier risk:
- Financial/liquidity/dilution:
- Regulatory/geopolitical:
- What would break the thesis:

## Trade Disclosure Status
[Explicit buy/long, hold/own, add, sell/reduce, no position, thesis-only, or unknown.]
```

## Basket Template

```markdown
| Candidate | Node | Chokepoint score | Evidence score | Mispricing score | Catalyst | Key risk | Confidence |
|---|---|---:|---:|---:|---|---|---|
```

## Evidence Priorities

Prefer primary/current sources in this order:

1. Company filings, annual reports, prospectuses, investor decks.
2. Earnings-call transcripts and management commentary.
3. Customer/vendor technical docs, qualification language, product pages.
4. Government subsidy, national-security, export-control, or supply-chain documents.
5. Standards bodies, patents, technical papers.
6. Reputable news and analyst excerpts.
7. Social posts only as leads, never as final proof.

## Common Failure Modes

- Confusing a great technology with a great stock.
- Treating total TAM as captured TAM.
- Ignoring dilution, ATM programs, debt, or working-capital needs.
- Assuming "supplier to Nvidia" means material revenue.
- Missing multi-source procurement and customer bargaining power.
- Treating a disclosed position as audited proof.
- Letting a stock move validate the thesis before the supply-chain evidence validates it.
