# Structured Problem Solving — The Consultant's Engine

This reference covers the end-to-end problem-solving methodology used at MBB firms. This isn't about frameworks — it's about the thinking process itself.

## Table of Contents
1. [Problem Definition](#problem-definition)
2. [Structuring the Problem](#structuring-the-problem)
3. [Hypothesis-Driven Approach](#hypothesis-driven-approach)
4. [Prioritization and 80/20](#prioritization-and-8020)
5. [Analysis Design](#analysis-design)
6. [Synthesis — The Hardest Part](#synthesis--the-hardest-part)
7. [Stress-Testing Your Answer](#stress-testing-your-answer)

---

## Problem Definition

The most common reason consulting engagements fail is solving the wrong problem. Invest disproportionate time here.

### The Situation-Complication-Question (SCQ) Framework

**Situation**: The stable, agreed-upon context. "We are a $500M specialty chemicals company with 15% market share in North America."

**Complication**: What changed or what's wrong. "Over the past 2 years, margins have declined from 22% to 14% while competitors have maintained theirs."

**Question**: The specific question to answer. "What is driving the margin erosion and what should we do to restore margins to 20%+ within 18 months?"

### Good vs. Bad Problem Statements

**Bad**: "How do we grow?" (Too vague — grow what? By how much? By when?)
**Good**: "How can we grow EBITDA from $50M to $75M within 3 years without acquisitions?"

**Bad**: "We need a digital strategy." (What does digital mean here? What problem does it solve?)
**Good**: "How can we reduce customer acquisition cost from $180 to $100 by digitizing our sales funnel?"

### Clarifying Questions to Ask

Always ask these before diving in:
1. What would success look like? (Quantify if possible)
2. What constraints exist? (Budget, timeline, organizational, regulatory)
3. What's been tried before? Why didn't it work?
4. Who are the key stakeholders and what do they care about?
5. What decisions will this analysis inform?
6. What's the timeline for action?

---

## Structuring the Problem

### Building Issue Trees

Start from the top question and decompose into sub-questions. Each level should be MECE.

**Rules for good issue trees**:
- Each branch should be answerable with analysis (not just "it depends")
- 2-4 branches at each level (more than 5 means you need a higher-level grouping)
- Go 3-4 levels deep maximum for the initial structure
- Label branches with questions, not topics ("Is volume declining?" not "Volume")

**Process**:
1. Write the key question at the top
2. Ask: "What are the 2-4 major components of this question?"
3. For each component, ask the same question
4. Stop when you reach a level where you can design a specific analysis

### Common Structuring Mistakes

- **Overlapping buckets**: "Marketing" and "Brand" as separate branches (not ME)
- **Missing categories**: Revenue tree that forgets pricing (not CE)
- **Too granular too fast**: Going to 6 levels before testing the top level
- **Framework worship**: Forcing Porter's 5 Forces onto a cost reduction problem
- **Topic trees instead of question trees**: Listing areas instead of hypotheses

### Custom vs. Standard Frameworks

**Use standard frameworks when**: The problem clearly maps to one (profitability decline → profit tree; market entry → 3C's + market sizing)

**Build custom structures when**: The problem is unique, crosses multiple domains, or standard frameworks force awkward fits

**How to build custom structures**: Start with the decision, work backward to what you need to know, group into MECE buckets. Name the buckets clearly.

---

## Hypothesis-Driven Approach

This is the single most important consulting technique. It's what separates a 2-week engagement from a 2-month research project.

### How It Works

1. **Day 1 Hypothesis**: Based on initial data and pattern recognition, form a point of view. "We believe the margin decline is driven by (a) input cost increases that weren't passed through in pricing and (b) a shift in customer mix toward lower-margin segments."

2. **Design analyses to test**: For each hypothesis:
   - What data would confirm it?
   - What data would disprove it?
   - What's the fastest way to get directional evidence?

3. **Prove, disprove, or pivot**: Run the analyses. The hypothesis is disposable — it's a tool for focusing effort, not a conclusion to defend.

### Why This Matters

Without a hypothesis, analysis becomes exploratory — "let's look at everything and see what we find." This is slow, expensive, and often produces volumes of data with no clear insight. The hypothesis focuses your attention on the 20% of analysis that drives 80% of the answer.

### The Ghost Deck / Storyboard

Before running any analysis, write the "ghost deck" — the final presentation with blank slides that have:
- Action titles (the insight each slide will convey)
- The chart or analysis that would prove the point
- Where the data will come from

This forces you to think about what you need to prove before you start analyzing. It prevents the common trap of "we ran a ton of analysis but can't figure out what it means."

Example ghost slide:
> **Title**: "Raw material costs increased 18% but pricing only increased 5%, creating a 13pp margin gap"
> **Analysis**: Waterfall chart showing margin bridge from Year 1 to Year 2
> **Data needed**: P&L line items by year, input cost index, pricing history

---

## Prioritization and 80/20

### Impact vs. Feasibility Matrix

Plot every potential initiative on:
- **Y-axis**: Impact (revenue, cost, strategic value)
- **X-axis**: Feasibility (cost, time, complexity, risk)

Quadrants:
- **Top-right**: Quick wins — do first
- **Top-left**: Major projects — plan carefully
- **Bottom-right**: Fill-ins — do if resources allow
- **Bottom-left**: Deprioritize — don't waste time

### The "Where to Play" Filter

When the issue tree has many branches, prioritize based on:
1. **Magnitude**: Which branch has the biggest potential impact?
2. **Data availability**: Where can we get evidence quickly?
3. **Actionability**: Can the client actually do something about it?
4. **Likelihood**: Based on pattern recognition, which hypotheses are most likely?

Spend 80% of your time on the top 2-3 branches. Have a point of view on the rest, but don't do deep dives.

### Pareto Analysis

In any problem, look for the Pareto pattern:
- Which 20% of customers drive 80% of revenue?
- Which 20% of SKUs drive 80% of profit?
- Which 20% of cost categories drive 80% of spend?
- Which 20% of defect types cause 80% of quality issues?

Start analysis at the concentrated end.

---

## Analysis Design

### The Analysis Plan

For each priority branch of the issue tree, specify:
1. **Hypothesis**: What do you expect to find?
2. **Analysis**: What analysis will test this?
3. **Data**: What data do you need?
4. **Source**: Where does the data come from?
5. **Owner**: Who will run this analysis?
6. **Timeline**: When will it be done?

### Types of Analyses

**Quantitative**:
- Trend analysis (is it getting better or worse?)
- Decomposition (what's driving the aggregate number?)
- Benchmarking (how does it compare to best-in-class?)
- Sensitivity analysis (what matters most?)
- Correlation analysis (what moves together?)
- Break-even analysis (when does this pay off?)

**Qualitative**:
- Expert interviews (internal and external)
- Customer research (surveys, interviews, focus groups)
- Competitive intelligence (public filings, trade press, expert networks)
- Best practice review (what do top performers do differently?)

### Analytical Rigor Checklist

Before presenting any analysis:
- [ ] Is the data source reliable?
- [ ] Are the assumptions explicit and reasonable?
- [ ] Does the conclusion follow from the evidence?
- [ ] Have I considered alternative explanations?
- [ ] Does it pass the smell test? (Is the magnitude reasonable?)
- [ ] Can I explain it simply to a non-expert?

---

## Synthesis — The Hardest Part

Synthesis is not summary. Summary says "here's what we found." Synthesis says "here's what it means and what to do."

### The Synthesis Process

1. **Lay out all findings**: What did each analysis show?
2. **Look for patterns**: What themes emerge across findings?
3. **Form the governing thought**: In one sentence, what's the answer?
4. **Build the argument**: What 2-4 points support the governing thought?
5. **Identify implications**: What should the client do differently?

### The "So What" Ladder

For every finding, climb the ladder:
- **Data point**: "Customer churn increased from 5% to 8%"
- **So what?**: "We're losing $15M in annual recurring revenue"
- **So what?**: "At this rate, we'll miss the revenue target by 12%"
- **So what?**: "We need to invest in retention now — the cost of replacing lost customers is 5x the cost of retaining them"
- **Recommendation**: "Launch a targeted retention program for top-quartile customers within 60 days"

### Synthesis Traps to Avoid

- **Data dump**: Presenting every analysis without a through-line
- **Balanced to a fault**: "There are pros and cons" — take a position
- **Recency bias**: Over-weighting the last analysis you ran
- **Confirmation bias**: Only seeing evidence that supports your hypothesis
- **Missing the forest**: Getting lost in details and missing the big picture

---

## Stress-Testing Your Answer

Before presenting any recommendation, run these tests:

### The "Hostile Board Member" Test
Imagine a skeptical board member who will challenge every assumption. Can you defend:
- Why this is the right problem to solve?
- Why your analysis is reliable?
- Why this recommendation over the alternatives?
- Why now? Why not wait for more data?

### The "CFO Test"
Can you quantify the impact? What's the NPV? What's the payback period? What's the risk-adjusted return? If you can't put a number on it, the recommendation is weak.

### The Sensitivity Analysis
What assumptions matter most? If input cost doesn't decline as projected, does the recommendation still hold? Test the 2-3 most critical assumptions and show the range of outcomes.

### The "Monday Morning" Test
If the CEO agrees with your recommendation, what do they do on Monday morning? If you can't answer this specifically, your recommendation isn't actionable enough.

### The Pre-Mortem
Assume the recommendation was implemented and failed. Why did it fail? The most common failure modes:
- Organizational resistance / lack of capability
- Competitive response that wasn't anticipated
- Market shift that invalidated assumptions
- Execution complexity underestimated
- Timeline unrealistic

Build mitigations for the top 2-3 failure modes into your recommendation.
