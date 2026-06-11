# Serenity Pattern Library

Use these archetypes as reusable patterns. Do not treat them as current recommendations.

## 1. Material Bottleneck of the Bottleneck

Pattern: end product depends on a substrate or chemical; the substrate depends on an even scarcer precursor.

Examples from the corpus:

- AXTI: InP substrate exposure for photonics.
- Nippon Chemical: high-purity phosphorus as an upstream input to InP substrates.

Reusable checks:

- Which material is physically required?
- Who controls purity, yield, or scale?
- Can customers qualify substitutes quickly?
- Does a tiny upstream revenue pool control a huge downstream buildout?

## 2. Architecture Transition Supplier

Pattern: a new architecture changes the component stack, creating winners that screeners do not recognize.

Examples:

- SIVE: lasers tied to CPO/pluggable optical transceiver architectures.
- FOCI: FAU/optical components tied to CPO mass production.
- Nextronics: CPO connectors and cage thermal modules.

Reusable checks:

- What changed in the architecture?
- Which old component becomes more valuable or newly mandatory?
- Is the supplier named in customer, technical, or analyst material?
- Is revenue still too small for conventional screens?

## 3. Seven-Layer Chokepoint Map

Pattern: map an AI supply chain as stacked failure points instead of a single supplier list. The goal is to find "the bottleneck inside the bottleneck."

Example layer map from the Serenity corpus:

1. Raw material: InP substrate inputs and specialty chemicals.
2. Crystal growth equipment: specialized crucibles/tools such as pBN-related equipment.
3. Substrate processing: substrate growers and processing oligopolies.
4. Light source: CW lasers and external light sources for CPO.
5. Optical module/system: AAOI, LITE, COHR, Innolight-type assemblers.
6. Test equipment: photonics and optical device test bottlenecks.
7. Fiber/cable: conventional and hollow-core fiber paths.

Reusable checks:

- What are the seven or fewer physical layers between demand and deployment?
- At each layer, what breaks if capacity is unavailable?
- Which layer is already crowded and which layer still lacks coverage?
- Which tiny upstream node can delay a much larger downstream revenue pool?
- Which layer becomes more important as architecture shifts from pluggables to CPO/ELS/SiPh?

## 4. Foundry / Packaging Capacity With Strategic Backstop

Pattern: an underappreciated manufacturing node becomes strategic because Western supply chains need domestic or allied capacity.

Examples:

- Shunsin: photonics packaging tied to Foxconn/AI hardware assembly.
- XFAB: SiC/GaN/MEMS/silicon photonics foundry capacity with US/EU subsidy signals.

Reusable checks:

- Is the company a foundry, packager, or equipment bottleneck rather than a product brand?
- Does government funding validate criticality?
- Is book value/replacement value low relative to strategic value?
- Are customers already qualifying the node?

## 5. Infrastructure Bottleneck Outside Semis

Pattern: AI/data-center growth moves the bottleneck away from chips into power, cooling, grid, or physical infrastructure.

Example:

- Hammond: transformers and switchgear bottleneck for data-center power infrastructure.

Reusable checks:

- Which physical infrastructure is delaying deployments?
- Are lead times multi-year?
- Does the candidate have capacity in the right geography?
- Can it price through raw-material inflation?
- Is backlog growth visible?

## 6. Forward-TAM / Low-Current-Revenue Mismatch

Pattern: current financials look small, messy, or cyclical, while future content per system may scale sharply.

Examples:

- IQE: epiwafers as upstream photonics supply.
- AAOI: Made-in-America optical transceiver/laser fab optionality.

Reusable checks:

- What is current revenue from the relevant segment?
- What future system volume drives content growth?
- Is the company constrained by dilution or capacity capex?
- Can it capture margin, or will customers extract the upside?

## 7. Small-Cap Demand Shock Translation

Pattern: a product or developer behavior shift is visible to everyone, but the market maps it to the obvious mega-cap instead of the small listed company whose financials can actually move.

Example:

- Raspberry Pi / RPI: OpenClaw-style local AI agent hardware demand could be noise for Apple but material for a small hardware company. The edge is not noticing the trend; it is translating the trend into company-level revenue acceleration, then comparing that with stale analyst expectations.

Reusable checks:

- What exactly changed in user behavior or procurement?
- Which listed company is small enough for the demand shock to matter?
- What part of revenue is exposed to the shock?
- Can unit demand be estimated from user behavior, channel checks, inventory, or reported segment data?
- Does the market still categorize the company under the old identity, such as education hardware, hobbyist product, or legacy industrial?
- Are consensus revenue growth, forward sales, or forward P/E still anchored to the old identity?
- What would prove the trend is only temporary?

## 8. Small-Cap Pricing Vacuum and Reflexivity

Pattern: the market ignores a small critical supplier because analysts and large funds cannot justify the work or cannot buy enough size. When evidence arrives, price discovery can be violent.

Examples:

- SIVE: small market cap, low liquidity, high strategic relevance, possible short-covering reflexivity.
- AXTI / AAOI: undercovered upstream/vertical integration names that rerated as the supply-chain role became visible.

Reusable checks:

- Is market cap below the threshold where large funds care?
- Is analyst coverage thin or stale?
- Is daily liquidity too small for institutions, creating a pricing vacuum?
- Is short interest material, and would positive evidence force buying?
- Could liquidity also trap holders on the way down?
- Does the thesis survive without a squeeze?

## 9. Institutional Rotation Pattern

Pattern: capital rotates through layers as the market digests a buildout. Serenity-style analysis tries to stand at the next layer before institutions arrive.

Example rotation:

- Stage 1: memory / HBM / obvious compute bottlenecks.
- Stage 2: optical modules and networking.
- Stage 3: external light sources, silicon photonics, substrates, test, packaging, and second-order suppliers.

Reusable checks:

- Which layer already rerated?
- Which adjacent layer must scale next?
- Which suppliers are still priced as legacy businesses?
- What evidence shows institutions have started moving into the next layer?
- Is the next layer large enough to matter and small enough to be mispriced?

## 10. Bayesian Conviction Update Pattern

Pattern: treat the thesis as a hypothesis, not a belief. Build a strong prior from physical supply-chain research, then update conviction as evidence arrives.

Workflow:

1. Define `H`: this company is a future bottleneck or disproportionate beneficiary.
2. Build the prior from BOMs, papers, filings, customer docs, market size, and capacity maps.
3. Act or watch before certainty when expected value is high, but size according to uncertainty.
4. Update on evidence:
   - Positive: customer qualification, backlog, revenue beat, subsidy, supply shortage, patent/process validation, higher ASP, index/listing inflow.
   - Negative: substitution, customer insourcing, failed ramp, margin compression, dilution, weak management, thesis-invalidating technical data.
5. Compare posterior conviction across candidates; rotate attention or capital toward the most active bottleneck only when evidence improves, not merely when price moves.

Reusable checks:

- What was the original thesis?
- Which evidence would be highly likely if the thesis were true?
- Which evidence would be highly likely if the thesis were false?
- Has new evidence changed the thesis or only the stock price?
- Is the posterior stronger than competing opportunities?

## 11. Disclosure and Confidence Pattern

Serenity-style posts often mix thesis, disclosure, and inference. Separate them:

- "I went long", "I took positions", "personally long": explicit trade/holding.
- "I own most, not all": basket disclosure, medium confidence.
- "favorite", "compelling", "bullish", "could rerate": thesis-only unless paired with disclosure.
- "when I went long last year": explicit but retrospective; timing is uncertain.

## 12. Anti-Pattern Checklist

Reject or heavily discount ideas where:

- The only edge is that a popular account mentioned it.
- The company is merely adjacent to a theme, not structurally required.
- The thesis cannot name the exact component/material/capacity node.
- The thesis stops at the first obvious winner instead of digging into second- and third-order constraints.
- Substitutes can be qualified quickly.
- The company captures little economics despite being in the chain.
- Dilution, debt, or poor governance can absorb the upside.
- The catalyst path is just "market will notice."
- The short-squeeze/low-float setup is stronger than the operating thesis.
