# Pricing Strategy: The Full Toolkit

Pricing is the highest-leverage lever in any P&L. A 1% improvement in price typically generates 3-5x more EBITDA impact than a 1% improvement in volume or a 1% reduction in variable costs. Yet it's systematically underinvested in most companies.

---

## The Three Pricing Approaches (and Their Limits)

**Cost-plus pricing:** Price = Cost × (1 + target margin). Simple, predictable, defensible internally. The problem: it's entirely inward-looking. It ignores what customers are willing to pay and what competitors charge. In competitive markets, cost-plus either over-prices (losing volume) or under-prices (leaving money on the table).

**Competitor-based pricing:** Price to win relative to alternatives. Useful when you're entering a market or when there's a clear reference price. The problem: it anchors you to competitors' pricing mistakes. If the market is collectively under-pricing, you under-price with it.

**Value-based pricing:** Price = share of the economic value you create for the customer. The theoretically correct approach. The problem: it requires you to understand customer value creation deeply, which most companies don't. When done well, it's the highest-margin pricing approach.

In practice, sophisticated pricing uses all three as inputs — value-based sets the ceiling, competitor-based establishes the reference range, cost-plus establishes the floor.

---

## Understanding Willingness to Pay

Willingness to pay (WTP) is the maximum price a customer will pay before choosing the next-best alternative. WTP varies by:
- Customer segment (enterprise vs. SMB vs. consumer)
- Use case (the value created in one application vs. another)
- Context (urgency, switching costs, alternatives)
- Relationship maturity

**How to measure WTP:**

*Van Westendorp Price Sensitivity Meter (best for new products/services):*
Survey customers with four questions:
1. At what price would this product feel too cheap (raising quality concerns)?
2. At what price would this product feel like a bargain?
3. At what price would this product feel expensive but still worth it?
4. At what price would this product feel too expensive to consider?

Plot the cumulative % curves for each response. Four intersections emerge:
- **Point of Marginal Cheapness (PMC):** Too cheap × Expensive curves intersect — lower bound of acceptable pricing
- **Point of Marginal Expensiveness (PME):** Too expensive × Cheap curves intersect — upper bound
- **Indifference Price Point (IPP):** Where Cheap × Expensive curves intersect — neutral point
- **Optimal Price Point (OPP):** Where Too Cheap × Too Expensive intersect — highest acceptance

The PMC-to-PME range is your acceptable price range. OPP is your anchor for initial pricing decisions.

*Conjoint analysis (best for established products with multiple attributes):*
Present customers with sets of product configurations (varying price, features, terms) and ask them to choose. Statistical analysis reveals the implicit weight customers place on each attribute including price. More sophisticated than Van Westendorp but requires larger sample and more setup.

*Direct competitive benchmarking:*
Map your price vs. competitor prices vs. the value differential. If you deliver 20% more value than Competitor A but price 5% below them, you're leaving significant money on the table.

---

## The Price Waterfall

Most B2B companies don't know their real selling price. List price and pocket price are often 25-40% apart.

**Mapping the waterfall:**
Start with list price and identify every discount layer:
1. Contractual discounts (negotiated annually, by segment or account size)
2. Volume rebates (paid at end of period based on purchase volume)
3. Promotional discounts (time-limited promotions)
4. Payment term discounts (early payment incentives — 2/10 net 30 means 36% annualized)
5. Off-invoice allowances (marketing development funds, co-op advertising, training support)
6. Distributor/channel margins (if applicable)
7. Returns and credits

*Example for a B2B software company:*
- List price: $100k
- Contractual discount (-20%): -$20k
- Volume rebate (-5%): -$5k
- Early payment discount (-2%): -$1.6k
- Implementation absorbed (-8%): -$8k
- **Pocket price: $65.4k** (35% below list)

The analysis question: where is value leaking that could be recovered? Typical opportunities:
- **Discount rationalization:** Are discounts correlated with deal size, strategic value, or risk — or are they just salespeople negotiating? If there's no pattern, you're giving away margin arbitrarily.
- **Off-invoice allowances:** Often untracked and unrecovered. Map them and tie them to specific outcomes (co-op allowances paid against measurable marketing activity).
- **Payment term arbitrage:** 2% for early payment sounds small but at scale it adds up. Model the cost and see if it's worth paying.

---

## Price Architecture

Price architecture is the structure of your pricing — tiers, bundles, usage bases — distinct from price levels.

**Good/Better/Best (versioning):**
Three tiers (basic, standard, premium) anchored by the premium tier. Anchoring effect: most customers choose the middle tier, but the premium tier's existence makes the middle tier feel reasonable. The premium tier also captures high-willingness-to-pay customers who would have paid more for the standard.

Designing tiers: the Good tier should feel complete but limited. The Better tier should feel like the obvious default. The Best tier should feel aspirational but justified.

**Usage-based pricing:**
Price per transaction, per unit consumed, per API call, per active user. Aligns your revenue with the value customers receive — which means customers pay more when they get more value. Reduces adoption barrier (low commitment to start) but creates revenue variability.

Best fit: when customer value scales clearly with usage, and when there's a simple, auditable usage metric. SaaS companies increasingly move here from seat-based pricing.

**Outcome-based pricing:**
You charge based on results delivered, not inputs consumed. The highest form of value-based pricing. Also the hardest to implement — requires clear outcome measurement, attribution agreement, and risk tolerance on both sides.

Best fit: when outcomes are clearly measurable, attributable to your product/service, and significant enough to share economically.

**Bundle vs. unbundle:**
Bundling combines multiple offerings at a discount to list — increases perceived value, reduces price sensitivity, raises switching costs (they're using multiple products). Unbundling separates offerings so customers only buy what they need — lowers adoption barrier, can reveal willingness to pay by component, often used to match a lower-cost competitor.

---

## Pricing Execution: Where Margin Leaks in Sales

The best pricing strategy fails if sales doesn't execute it. The most common execution failures:

**Undisciplined discounting.** Sales reps offer discounts reactively (when the customer asks) rather than strategically (when it's necessary to close a deal that wouldn't otherwise close). Fix: implement a discount approval matrix — small discounts pre-approved, larger discounts require management sign-off. Track discount rate by rep and make it visible.

**No price discipline on renewals.** Acquiring new customers at better pricing than renewing existing ones. Fix: price increases on renewals should be planned and systematic — not a surprise to the customer, not an afterthought to the sales team.

**No value anchoring before price.** Salespeople discussing price before establishing value context. Fix: train sales to quantify economic value created before introducing price. "You'll save X hours per week across your 50 analysts at $Y per hour loaded cost — that's $Z per year. Our pricing is..." frames the conversation very differently.

**Ignoring competitive price response.** When a competitor drops price, the reflexive response is to match. Often this is wrong — price wars destroy value for everyone. Before matching, ask: Is this competitor move rational? Can they sustain it? What's our value differential that justifies our premium?

---

## Pricing Diagnostics: Where to Start

When diagnosing a pricing problem, run these analyses in sequence:

1. **Build the price waterfall** — understand realized vs. list price by segment and channel
2. **Analyze discount patterns** — correlation of discount depth with deal size, rep, segment, sales cycle length
3. **Compare realized price vs. value delivered** — are you capturing an appropriate share of value?
4. **Benchmark vs. competitors** — are you priced appropriately for your value positioning?
5. **Analyze price elasticity** — what happened to volume when you raised/lowered prices historically?
6. **Assess architecture fit** — is your pricing structure aligned with how customers derive value?

Most companies find their biggest opportunity in steps 2 and 3: margin leaking through undisciplined discounting, and systematic under-pricing relative to value delivered.
