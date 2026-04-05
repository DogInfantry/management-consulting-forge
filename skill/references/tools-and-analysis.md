# Analytical Tools & Quantitative Methods

This reference covers the quantitative toolkit every management consultant needs: financial analysis, data analysis, modeling, and the math behind common consulting analyses.

## Table of Contents
1. [Financial Analysis Toolkit](#financial-analysis-toolkit)
2. [Operational Analysis](#operational-analysis)
3. [Statistical and Data Analysis](#statistical-and-data-analysis)
4. [Scenario and Sensitivity Analysis](#scenario-and-sensitivity-analysis)
5. [Common Calculations and Formulas](#common-calculations-and-formulas)
6. [Excel / Modeling Best Practices](#excel--modeling-best-practices)

---

## Financial Analysis Toolkit

### P&L Disaggregation
Always start by breaking the P&L into its components and analyzing trends:

```
Revenue
  - by product/service line
  - by customer segment
  - by geography
  - by channel
(-) COGS
  - materials
  - labor
  - overhead
  - depreciation
= Gross Profit (and Gross Margin %)

(-) SGA
  - sales & marketing
  - general & administrative
  - R&D
= EBITDA (and EBITDA Margin %)

(-) D&A, Interest, Tax
= Net Income
```

For each line: What's the trend? What's driving it? How does it compare to benchmarks?

### Revenue Decomposition
```
Revenue = Volume × Price
Volume = Customers × Frequency × Units per Transaction
Price = List Price × (1 - Discount Rate) × Mix Effect

Revenue Growth = Volume Growth + Price Growth + Mix Effect
```

### Margin Bridge / Waterfall
Show what drove margin change from Period A to Period B:

```
Period A Margin: 25%
+ Price improvement: +2pp
+ Input cost reduction: +1pp
- Volume deleverage: -1.5pp
- SGA increase: -0.5pp
- Mix shift: -1pp
= Period B Margin: 25%
```

### Break-Even Analysis
```
Break-Even Volume = Fixed Costs / Contribution Margin per Unit
Contribution Margin = Price - Variable Cost per Unit

Break-Even Revenue = Fixed Costs / Contribution Margin %
```

Use for: New product launches, investment decisions, pricing decisions, capacity additions.

### Working Capital Analysis
```
Cash Conversion Cycle = DSO + DIO - DPO

DSO (Days Sales Outstanding) = (Receivables / Revenue) × 365
DIO (Days Inventory Outstanding) = (Inventory / COGS) × 365
DPO (Days Payable Outstanding) = (Payables / COGS) × 365
```

Improvement opportunity = Closing the gap to best-in-class × daily cash flow impact.

### Return on Investment Metrics
```
ROI = (Net Benefit / Cost) × 100%
Payback Period = Investment / Annual Net Cash Flow
NPV = Σ [Cash Flow_t / (1 + r)^t] - Initial Investment
IRR = Rate where NPV = 0
```

**Decision rules**: NPV > 0 → invest. IRR > hurdle rate → invest. Payback < threshold → invest.

### DCF Valuation
```
Enterprise Value = Σ [UFCF_t / (1 + WACC)^t] + Terminal Value / (1 + WACC)^n

UFCF = EBIT × (1 - Tax Rate) + D&A - Capex - ΔWorking Capital

Terminal Value = UFCF_terminal × (1 + g) / (WACC - g)
  where g = long-term growth rate (typically 2-3%)

WACC = (E/V × Re) + (D/V × Rd × (1-T))
  Re = Rf + β × (Rm - Rf)    [CAPM]
```

Key sensitivity variables: Revenue growth, EBITDA margin, WACC, terminal growth rate.

---

## Operational Analysis

### Process Mapping & Throughput
```
Throughput = 1 / Bottleneck Cycle Time
Capacity Utilization = Actual Output / Maximum Output
OEE = Availability × Performance × Quality
```

### Procurement Savings Levers
1. **Volume consolidation**: Combine spend across categories/locations for volume discounts
2. **Specification optimization**: Reduce over-specification without affecting quality
3. **Supplier switching**: Competitive bidding drives down prices
4. **Demand management**: Reduce consumption (do we need this at all?)
5. **Total cost of ownership**: Include logistics, quality, lead time — not just unit price

**Typical savings by lever**: 5-15% on direct materials, 10-25% on indirect/services.

### Benchmarking Methodology
1. **Select metrics**: Choose 5-10 KPIs that matter for the problem
2. **Define peer set**: Best-in-class (aspirational), direct competitors (competitive), and industry median (baseline)
3. **Collect data**: Public filings, industry reports, expert interviews
4. **Analyze gaps**: For each metric, how far is the client from best-in-class?
5. **Size the prize**: Convert gaps to financial impact (e.g., "closing the inventory turns gap from 6x to 9x would free $40M in cash")

### Customer / Product Profitability
Often 20% of customers/products drive 80%+ of profit, and some customers/products are actually unprofitable.

```
Customer Profitability = Revenue from Customer
                        - Direct costs to serve
                        - Allocated overhead (activity-based)
                        = Customer Profit

Sort customers by profitability → create whale curve (cumulative profit chart)
```

Typical finding: The top 20% of customers generate 150-200% of total profit, and the bottom 20% destroy 50-100% of it.

---

## Statistical and Data Analysis

### Regression Basics
For identifying drivers and predicting outcomes:
- **Simple linear**: y = mx + b (one predictor)
- **Multiple**: y = b₀ + b₁x₁ + b₂x₂ + ... (multiple predictors)
- **R²**: % of variation explained (>0.7 is generally good for business data)
- **p-value**: <0.05 means statistically significant

Use cases: What drives customer churn? What predicts sales performance? What causes cost variation?

### Cohort Analysis
Track groups of customers (cohorts) over time to understand retention, spending patterns, and LTV. Essential for subscription businesses and any recurring revenue model.

```
Month 0: 1,000 new customers
Month 1: 850 still active (85% retention)
Month 3: 700 still active (70% retention)
Month 12: 450 still active (45% retention)
→ Average monthly churn: ~5.5%
→ Expected lifetime: ~18 months
→ LTV = Monthly revenue × Margin × 18
```

### Segmentation Analysis
Divide a population into meaningful groups using:
- **RFM Analysis**: Recency (when last purchase), Frequency (how often), Monetary (how much)
- **Needs-based**: What do they value? (price, quality, convenience, service)
- **Behavioral**: How do they buy? (online/offline, impulse/considered, brand loyal/switcher)
- **Value-based**: High-value vs. low-value customers

### A/B Testing Framework
For any intervention (pricing change, marketing campaign, process improvement):
1. **Hypothesis**: What do you expect to happen?
2. **Test design**: What's the control? What's the treatment? How long to run?
3. **Sample size**: Need enough data for statistical significance
4. **Metric**: What are you measuring? (primary and secondary metrics)
5. **Analysis**: Is the difference statistically significant? Practically significant?

---

## Scenario and Sensitivity Analysis

### Scenario Analysis
Build 3 scenarios for any forecast or business case:

| | Base Case | Upside | Downside |
|--|-----------|--------|----------|
| **Probability** | 50-60% | 20-25% | 20-25% |
| **Revenue growth** | 8% | 15% | 2% |
| **Margin** | 18% | 22% | 12% |
| **NPV** | $45M | $78M | $12M |
| **Key assumption** | Market grows at historical rate | Win key account + pricing power | Recession + competitive entry |

### Sensitivity Analysis (Tornado Chart)
Test the impact of changing each input ±20%:

```
Variable          | -20% Impact | +20% Impact | Range
Volume growth     |   NPV $25M  |   NPV $65M  |  $40M  ← Most sensitive
Pricing           |   NPV $30M  |   NPV $60M  |  $30M
COGS %            |   NPV $50M  |   NPV $40M  |  $10M
Capex             |   NPV $48M  |   NPV $42M  |   $6M  ← Least sensitive
```

Focus risk mitigation on the most sensitive variables.

### Monte Carlo Simulation (Conceptual)
When you need to model multiple uncertain variables simultaneously:
1. Define probability distributions for key inputs
2. Run thousands of simulations
3. Output: probability distribution of outcomes
4. Use to answer: "What's the probability that NPV > 0?" or "What's the 90th percentile downside?"

---

## Common Calculations and Formulas

### Growth Rates
```
YoY Growth = (Current - Prior) / Prior × 100%
CAGR = (End Value / Start Value)^(1/n) - 1
Rule of 72: Years to double = 72 / Growth Rate %
```

### Weighted Average
```
Weighted Average = Σ (Value_i × Weight_i) / Σ Weight_i
```
Use for: WACC, weighted customer satisfaction, blended margins.

### Index Numbers
Set a base period = 100, express subsequent periods as % of base.
Useful for comparing growth across items with different absolute values.

### Market Share
```
Market Share = Company Revenue / Total Market Revenue
Relative Market Share = Company Share / Largest Competitor's Share
```

### Elasticity
```
Price Elasticity = % Change in Quantity / % Change in Price
```
- Elastic (|E| > 1): Demand is sensitive to price (reduce price to grow revenue)
- Inelastic (|E| < 1): Demand is stable (can raise price with limited volume loss)
- Typical: Consumer staples (0.3-0.6), Consumer discretionary (1.0-2.5), Luxury (0.5-0.8)

---

## Excel / Modeling Best Practices

### Model Structure
- **Inputs** (blue font): All assumptions in one place, clearly labeled
- **Calculations** (black font): Formulas only — never hardcode numbers in calculation cells
- **Outputs** (green or bold): Summary results and key metrics

### Golden Rules
1. **One formula per row**: Every row uses the same formula across all columns
2. **No circular references**: These are errors, not features
3. **Separate inputs from calculations**: Makes sensitivity analysis trivial
4. **Label everything**: Units, time periods, sources
5. **Build in error checks**: Do assets = liabilities + equity? Does cash flow tie?
6. **Use scenarios**: Toggle between base/upside/downside with a single input cell

### Common Model Types
- **3-Statement Model**: Income statement → Balance sheet → Cash flow, all linked
- **DCF Model**: 3-statement + free cash flow + discount + terminal value
- **LBO Model**: 3-statement + debt schedule + returns analysis
- **Operating Model**: Driver-based forecast of revenue and costs by business unit
- **Unit Economics Model**: Revenue, cost, and margin at the customer/product level
