# Quantitative Toolkit for Management Consulting

A sharp 3-4 year MBB consultant's practical guide to the math that shows up on nearly every engagement.

## 1. Back-of-Envelope Sizing

You have 10 minutes. No model. No primary research. Get to a useful number.

**Three approaches:**

**Top-down market sizing:**
Start with something you know. US GDP ~$28T. US adult population ~260M. Work down to your addressable market.

Example: "What's the market for cloud spend in manufacturing?"
- US manufacturing revenue: ~$2.3T
- Assume 10% of manufacturing costs go to IT: $230B
- Cloud penetration in mfg: assume 20% of that: $46B
- By 2030, assume 40% penetration: $92B

**Bottom-up unit sizing:**
Units times price. Forces you to think operationally.

Example: "What's the US restaurant market?"
- ~660k restaurants in US
- Average revenue per restaurant: ~$1.2M (median much lower; this is skewed by chains)
- Total: ~$790B

**Analog-based:**
Find something similar in another geography or time period.

Example: "What's India's e-commerce opportunity?"
- Brazil's e-commerce: ~5% of retail
- Brazil's per capita income: ~$8.5k
- India's per capita income: ~$2.3k; adjust down to 2% of retail
- India's retail market: ~$700B
- India's e-commerce: ~$14B

**Sanity checks:**
- Revenue ÷ population. If you estimated $1T market for US adult software and got $5k per person, flag it.
- Ratio to something public. If your restaurant estimate implies $1.2M average check, you broke something.
- Work backwards. If enterprise SaaS is $200B market and you estimate 40M SMB accounts at $50/month each, that's only $24B. Mismatch signals error.

**Numbers to memorize:**
- US GDP: $28T
- US adult population: 260M
- US household income (median): $74k
- US household income (average): $110k
- Global GDP: $110T
- China GDP: $18T
- Europe GDP (EU): $17T
- Corporate COGS typically: 40-60% of revenue (varies wildly by sector)
- SG&A for B2B: 30-50% of revenue
- R&D for tech: 15-30% of revenue

When does back-of-envelope stop working? When the number drives a major decision and you need ±20% confidence. Then you model.

## 2. Unit Economics

The fastest way to understand if a business works.

**Start with the basics:**

**Customer Acquisition Cost (CAC):**
Sales and marketing spend ÷ number of new customers acquired in that period.
- Don't use annual CAC across a seasonal business.
- If you have channels (field sales vs. inside sales vs. SMB vs. enterprise), calculate CAC by channel.
- CAC from company P&L: Sales & Marketing / Customer Acquisition (from operational data, not assumptions).

**Lifetime Value (LTV):**
Gross profit per customer × lifetime in years.

LTV = (Average Contract Value × Gross Margin %) / (Monthly Churn Rate)

For a SaaS company with $10k ACV, 80% gross margin, 2% monthly churn:
LTV = ($10k × 0.80) / 0.02 = $400k

**LTV/CAC Ratio:**
The magic number. Healthy is 3:1 or better. Anything below 2:1, you're buying customers too expensively.
- If LTV/CAC = 5:1, you're underspending on acquisition.
- If ratio is declining YoY with no strategy shift, something is breaking.

**Payback Period:**
How long until the CAC is recovered from gross profit. (CAC) ÷ (Gross Profit per Customer per Month).

CAC $50k, monthly gross profit per customer $2k: 25-month payback. That's slow for SaaS (typical: 12-18 months).

**Contribution Margin:**
Revenue minus all variable costs (COGS, customer support, payment processing, etc.). As a % of revenue.

If CM% is 30%, you cover 30% of fixed costs and profit from each incremental sale. Use this for breakeven analysis.

**Gross Margin:**
(Revenue - COGS) / Revenue. COGS is pure product cost. For SaaS, this is hosting, support, refunds. For hardware, manufacturing.

At 80% gross margin, you can afford 40% SG&A and still be profitable at scale.

**What healthy looks like:**
- B2B SaaS: 75%+ gross margin, LTV/CAC > 3:1, 12-18 month payback
- E-commerce: 45%+ gross margin (before fulfillment), LTV/CAC > 2:1
- Marketplace: 60%+ take rate, LTV/CAC > 2:1
- B2B services: 50%+ contribution margin (after delivery), CAC payback < 12 months

**Warning signs:**
- LTV/CAC < 1.5:1 with no clear path to improve
- Churn accelerating (suggests unit economics are deteriorating)
- CAC rising while LTV flat (math breaks down)
- Gross margin < 40% in capital-light business (structural problem)

Connect to strategy: If LTV/CAC is 2:1 and your market is expanding 30%, you might decide to spend more on acquisition. If it's 5:1 and the market is mature, you're not efficient.

## 3. Benchmarking Methodology

A benchmark study is only as good as your peer set and your data cleaning.

**Selecting peers:**

Ask first: what dimension are you benchmarking on? Operating margin? Customer acquisition cost? Organizational span? Peers must be comparable on that dimension.

- **By revenue size**: Useful when you're asking "are our costs in line?" Peer set: ±30% of your revenue.
- **By business model**: Useful when comparing operational KPIs. Subscription vs. perpetual is very different. B2B vs. B2C is very different.
- **Best-in-class regardless of size**: Useful for "what's possible?" You might benchmark a 2-person finance team against a 500-person company's finance team to show you're overstaffed.

**Normalizing for comparability:**

Raw numbers lie. Always normalize.

Example: You have 5 competitors' cost data.
- Competitor A: $20M SG&A, $100M revenue → 20% of revenue
- Competitor B: $35M SG&A, $140M revenue → 25% of revenue
- Competitor C: $8M SG&A, $50M revenue → 16% of revenue

Now compare: Competitor C is most efficient. But is it a smaller, scrappier company? Did it outsource support? Be skeptical before declaring it "best practice."

Cost as % of revenue works for everything. For headcount: measure as cost per revenue dollar, headcount per $1M revenue, or headcount per customer.

**Getting data when it's not public:**

- **Public companies**: Use 10-K filings. Build a model with 10-15 comparable companies.
- **Private companies**: If they've fundraised, check Crunchbase or PitchBook for revenue ranges. Call their sales team. Talk to customers.
- **Industry reports**: Gartner, IDC, proprietary databases. Expensive, worth it.
- **Best practice**: Run a survey. "We're studying cost structures; would you share anonymized data in exchange for a custom benchmark?" Get 8-12 responses, take the 25th-75th percentile.

**Presenting gaps without over-interpreting:**

Say: "Peer set median SG&A is 28% of revenue; you're at 34%. This suggests either (a) higher service levels, (b) inefficiency, or (c) different revenue mix. Here's what I see…"

Do NOT say: "You're overspending by 6% of revenue." You don't know that yet.

Show ranges (25th-75th percentile), not just median. Show what drives outliers. A peer at 18% SG&A probably outsourced support; one at 45% is early-stage and investing in growth.

## 4. Price Waterfall Analysis

Most companies don't know their real selling price.

List price and realized price are often 30-50% apart.

**Map every discount layer:**

Starting with list price, what gets deducted?

1. **Contractual discounts**: "Enterprise accounts get 20% off list."
2. **Volume rebates**: "If you hit $10M annual spend, you get an additional 5% back."
3. **Payment terms discounts**: "2% if you pay in 10 days." (Early payment discount = 36% annualized rate; companies take it all the time.)
4. **Off-invoice allowances**: Marketing development funds (MDF), training, implementation costs you absorb.
5. **Distributor/channel margins**: If selling through distributors, you're getting wholesale price.
6. **Returns/credits**: Assume ~2-5% of revenue.

Example: Enterprise software
- List price: $1M
- Contractual discount (20%): -$200k
- Volume rebate (5%): -$50k
- Early payment discount (2% taken): -$16k
- Implementation absorbed by you: -$50k
- **Pocket price: $684k** (32% below list)

That gap matters. If you're analyzing pricing power or competitive position, realized price is the only number that counts.

**Where value leaks:**

Look for:
- Discounts increasing year-over-year without volume corresponding increase (margin erosion)
- Distributor mix growing (automatic margin decline)
- Off-invoice allowances that are never reconciled (sink for value)
- Early payment discounts taken but never planned for (working capital hit)

**Fixing it:**

You can't just raise list price without addressing discounts. Pick one:
- Reduce contractual discounts (requires renegotiation; good for new deals)
- Reduce off-invoice allowances (requires saying no; risky)
- Shift to higher-margin channels (takes time)
- Volume-based pricing (structure that rewards scale and reduces discounting)

Pocket price analysis is how you find $20-50M in hidden margin.

## 5. Spans and Layers Analysis

The standard org efficiency diagnostic. Takes 2 hours. Usually reveals 15-25% cost opportunity.

**Map the layers:**

From CEO down, how many levels until front-line? Typical healthy org has 4-6 layers for 500-1k person company.

CEO → VP → Director → Manager → Individual Contributor.

**Calculate spans:**

Span = direct reports per manager.

Go through the org. Pick 20 managers at random. Average their direct reports.

- Healthy operational function (fulfillment, operations): 7-9 direct reports
- Healthy knowledge work (engineering, finance): 5-7 direct reports
- Complex coordination (sales): 4-6 direct reports (more complex deals = fewer reports)

Example: You have 300 people in operations. CEO → VP Ops → 5 Directors → 25 Managers → 270 ICs.

VP has span of 5 (good). Directors have span of 5 (tight for ops; should be 7-8). Managers have span of ~11 (good).

**Identifying inefficiency:**

Ask:
1. Are there more layers than necessary? (Cost of an extra layer: 3-5% of ops cost)
2. Are spans too tight? (Each tight span adds cost without scaling control)
3. Are there specialized roles that don't need to be there? (Program managers for a 30-person team)

If your org has 6 layers and a peer's has 4, that's 2 × 3% = ~6% cost opportunity.

**Structural redesign impact:**

Removing one layer = reduce headcount 10-15% in management. Actual savings is usually 5-8% due to realignment and some role expansion.

Increasing manager spans from 5 to 7 = reduce management cost 25-30% but usually need more individual contributors to handle exceptions.

**Benchmarks by function:**
- Sales: 4-5 span (complex deals, coaching needed)
- Customer success: 6-8 span (more scalable)
- Operations: 7-10 span (more process-driven)
- Finance: 5-7 span (medium complexity)
- IT/Shared services: 8-10 span (standardized tasks)

## 6. Sensitivity and Scenario Modeling

Executives want ranges, not point estimates. Build them properly.

**Find the 2-3 drivers:**

You've built a 5-year model with 50 assumptions. Which 3 matter most?

Use tornado analysis: vary each assumption ±20%, see which one moves the output most.

Usually it's:
1. Customer acquisition rate (drives revenue growth)
2. Churn rate (drives customer base)
3. Price/ARPU (drives margin)

Other stuff usually plays a minor role.

**Build a sensitivity table:**

Not a Monte Carlo simulation. A clean 3×3 table.

Example: 5-year EBITDA margin forecast

|  | Low Churn (1%) | Base Churn (2%) | High Churn (3%) |
|---|---|---|---|
| **Conservative Growth (15% CAC)** | 28% | 24% | 19% |
| **Base Growth (20% CAC)** | 32% | 27% | 21% |
| **Aggressive Growth (25% CAC)** | 36% | 30% | 23% |

This is readable. It shows the range (19-36%). Executive immediately sees "if churn goes to 3%, we're in trouble."

**Define scenarios meaningfully:**

Not just ±10% on everything. Real strategic uncertainty.

- **Base case**: Best guess, documented assumptions
- **Bull case**: What if competitive advantage holds? What if customer concentration risk doesn't materialize? (Usually 30-50% upside)
- **Bear case**: What if largest customer leaves? What if churn accelerates? (Usually 30-50% downside)

The bear case should be "ugly but survivable," not "apocalypse." If bear case shows bankruptcy, you haven't defined a real scenario; you've just scared people.

**Presenting without losing credibility:**

Say: "Our base case assumes 18% growth and 2% churn, giving us $X EBITDA by 2030. The range is $Y to $Z depending on market adoption and churn. Here are the key decision points that would shift us toward the bull or bear case."

Do NOT say: "We could be worth anywhere from $0 to $1B."

Show what drives movement between scenarios. Show when you'd revise. "If Year 2 churn exceeds 2.5%, we'll assume bull case is off and reduce growth guidance."

## 7. Reading a P&L for Signals

First time you open a P&L, 60 seconds. Calculate 4 ratios and flag year-over-year changes.

**Immediate calculations:**

1. **Gross margin**: (Revenue - COGS) / Revenue. Signals pricing power and cost structure.
2. **EBITDA margin**: (Revenue - OpEx - COGS) / Revenue. Real operating efficiency.
3. **SG&A as % of revenue**: Operating leverage. Is it dropping or stuck?
4. **R&D as % of revenue**: Growth investment. Increasing suggests growth mode; decreasing suggests maturity.

**Year-over-year flags:**

- Gross margin down 2+ points: Pricing pressure or cost inflation. Which?
- SG&A rising faster than revenue: Not scaling ops. Why?
- R&D constant in absolute $ but down as %: Underinvesting relative to growth.
- Headcount up 30%, revenue up 10%: Hiring ahead of revenue. Usually unsustainable.

**What the P&L won't tell you:**

- Cash flow (check the cash flow statement)
- Working capital changes (tie to balance sheet)
- Quality of earnings (check capex, one-time items, accounting changes)
- Customer concentration (check MD&A or segments)
- Payroll composition (check hiring data, not just OpEx)

**The move:**

Get the P&L. Calculate ratios. Ask: "Why did gross margin move? Why is SG&A % changing? Is this planned or a warning signal?" Usually within 30 minutes you've identified 2-3 hypotheses to test operationally.

---

**Last note:** These are tools, not answers. Use them to ask better questions. The consultant who can quickly size a market, spot margin erosion, or map an org is useful. The one who can then say "which of these three opportunities matters most to the business right now?" is a partner.
