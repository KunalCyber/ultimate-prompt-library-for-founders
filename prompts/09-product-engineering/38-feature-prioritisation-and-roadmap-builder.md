# Feature Prioritisation and Roadmap Builder

**Domain:** Product and Engineering
**Level:** 🔵 Practitioner

> Prioritise your feature backlog using a structured scoring framework and produce a phased product roadmap. Replaces gut-feel prioritisation with a defensible, documented process.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_NAME]` | Name of the product | e.g. ComplianceOS |
| `[BACKLOG_ITEMS]` | List your backlog items | e.g. (1) Auto evidence collection, (2) FCA horizon scanning alerts, (3) Board reporting dashboard, (4) Multi-user permissions, (5) Audit trail export, (6) GDPR module, (7) API for third-party integrations, (8) Mobile app |
| `[BUSINESS_GOAL]` | The primary business goal for the next 6 months | e.g. Reach 10 paying customers and £180k ARR; current customers need evidence collection and reporting features to renew |
| `[TEAM_CAPACITY]` | Engineering capacity available | e.g. 1 full-stack engineer, 8 weeks per quarter, estimated 3-5 days per feature depending on complexity |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a product director with 15 years of experience prioritising roadmaps for B2B SaaS companies. You have a disciplined, framework-driven approach to prioritisation and zero patience for HiPPO-driven roadmaps (Highest Paid Person's Opinion). Every feature on the roadmap earns its position through evidence and scoring, not internal advocacy.
</role>

<context>
Product name: [PRODUCT_NAME]
Backlog items: [BACKLOG_ITEMS]
Business goal: [BUSINESS_GOAL]
Team capacity: [TEAM_CAPACITY]
</context>

<instructions>
Step 1: Score each backlog item across five dimensions: Customer Value (how much does this improve the customer experience?), Revenue Impact (how directly does this drive new revenue or retention?), Strategic Fit (how well does this align with the stated business goal?), Implementation Effort (how complex is this to build?), Risk Reduction (does this reduce compliance, technical, or business risk?). Score 1-5 on each.

Step 2: Apply a weighting to each dimension based on the stated business goal. Weights must sum to 100%.

Step 3: Calculate weighted scores and rank the backlog.

Step 4: Assign each item to a roadmap phase: Now (Q1), Next (Q2), Later (Q3-Q4), or Backlog (deprioritised). Phases must be consistent with stated team capacity.

Step 5: Produce a one-paragraph rationale for the top three prioritised items explaining why they rank above the rest.
</instructions>

<output_format>
Section 1: Scoring Matrix. Rows: each backlog item. Columns: Customer Value, Revenue Impact, Strategic Fit, Effort (inverted: low effort = high score), Risk Reduction, Weighted Score, Rank.
Section 2: Dimension Weights. Table with Dimension, Weight, and Rationale for Weight columns.
Section 3: Phased Roadmap. Four columns (Now/Next/Later/Backlog) with items assigned to each phase. Include estimated effort per item.
Section 4: Top Three Rationale. Three numbered paragraphs, one per top-ranked item.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Dimension weights must sum to exactly 100%.
- Weighted scores must be mathematically correct.
- Effort scoring must be inverted: high effort = low score.
- Roadmap phases must respect stated team capacity. Do not put 8 features in the Now column for a 1-person team.
- Rationale must reference the scores, not just describe the feature.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Dimension weights sum to 100%.
2. Weighted scores are mathematically correct for each item.
3. Effort scores are inverted correctly.
4. Now column is feasible within stated team capacity.
5. Top three rationale references specific scores and business goal alignment.
</evaluation_criteria>
```

---

## Why This Works

The inverted effort scoring is the most commonly missed element in prioritisation frameworks. Features that are easy to build often score artificially low on effort because teams score 1 for easy and 5 for hard, then include effort in a sum rather than inverting it. Explicitly requiring inversion prevents the bias toward complex, high-prestige features that engineers prefer but customers may not need.

---

## Sample Output

Scoring row: Auto Evidence Collection | Customer Value: 5 | Revenue Impact: 5 | Strategic Fit: 5 | Effort (inverted): 2 (high complexity = low score) | Risk Reduction: 4 | Weighted Score: 4.3 | Rank: 1 | Note: ranks first despite high effort because the business goal is explicitly renewal-driven and this is the feature both current customers need to renew

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
