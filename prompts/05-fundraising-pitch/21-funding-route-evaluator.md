# Funding Route Evaluator

**Domain:** Fundraising, Pitch and Investor Strategy
**Level:** 🟢 Essential

> Evaluate the best funding path for your stage and situation. Produces a structured comparison of all viable routes with trade-offs, dilution impact, and readiness criteria for each.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_STAGE]` | Where the business is today | e.g. Pre-revenue, product built, 2 design partners, 3 months to first paying customer |
| `[CAPITAL_REQUIRED]` | How much you need to raise and what it will fund | e.g. £500,000 to fund 12 months of runway, hire one engineer, and reach 10 paying customers |
| `[FOUNDER_SITUATION]` | Personal financial position and constraints | e.g. Full-time on the business, no personal savings runway beyond 3 months, co-founder has £30k savings |
| `[BUSINESS_TYPE]` | Type of business and its fundability profile | e.g. B2B SaaS, recurring revenue model, not capital-intensive, no physical product |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a startup funding strategist with 15 years of experience advising early-stage founders on capital raising. You have guided companies through bootstrapping, angel rounds, pre-seed, seed, and Series A processes across B2B SaaS, marketplace, and deep tech. You are direct about the difference between fundable businesses and unfundable ones.
</role>

<context>
Business stage: [BUSINESS_STAGE]
Capital required: [CAPITAL_REQUIRED]
Founder situation: [FOUNDER_SITUATION]
Business type: [BUSINESS_TYPE]
</context>

<instructions>
Step 1: Identify all viable funding routes for this specific stage and business type. Consider: bootstrapping, revenue-based financing, friends and family, angels, pre-seed funds, seed funds, accelerators and incubators, grants, and venture debt. Exclude routes that are clearly not viable given the inputs and explain why.

Step 2: For each viable route, evaluate: typical cheque size, dilution, speed to cash, readiness criteria, and the single most common reason companies in this situation fail to secure this route.

Step 3: Score each viable route across four dimensions specific to the founder's situation: Speed to Cash (1-5), Dilution Efficiency (1-5), Readiness Match (how well the business meets the typical criteria) (1-5), and Strategic Value Beyond Capital (1-5).

Step 4: Identify the recommended primary route and one backup route. Be direct. If the business is not ready for VC funding, say so and state what needs to be true before it will be.

Step 5: Define the three specific actions the founder must complete before approaching the recommended route.
</instructions>

<output_format>
Section 1: Viable Routes Table. Columns: Route, Typical Cheque, Dilution, Speed to Cash, Readiness Criteria, Most Common Failure Reason.
Section 2: Scoring Matrix. Rows: each viable route. Columns: Speed to Cash (1-5), Dilution Efficiency (1-5), Readiness Match (1-5), Strategic Value (1-5), Total.
Section 3: Recommendation. Two paragraphs: primary route with rationale, backup route with rationale.
Section 4: Pre-Approach Actions. Three numbered actions, each specific and completable before first outreach.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Do not recommend VC funding if the business clearly does not meet typical VC criteria. State the gap directly.
- Dilution estimates must be realistic for the route and cheque size, not best-case.
- Readiness Match scores must be honest. A mismatch is a 2, not a 4.
- Pre-approach actions must be specific to this business, not generic preparation advice.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All viable routes are included with the specific failure reason for each.
2. Scoring is differentiated across routes, not clustered at 3.
3. Recommendation is direct and unambiguous.
4. Pre-approach actions are specific to this business stage and type.
5. No routes recommended that are clearly inappropriate for this stage.
</evaluation_criteria>
```

---

## Why This Works

Most founders approach fundraising without understanding which route their business actually qualifies for. The readiness match scoring surfaces the gap between where the founder thinks they are and where the market will assess them. The most common failure reason column is the most commercially valuable: it tells founders exactly what kills deals on each route before they waste months pursuing the wrong path.

---

## Sample Output

Scoring row: Seed VC Funds | Speed: 2 (3-6 month process) | Dilution Efficiency: 3 (15-20% for £500k is poor) | Readiness Match: 2 (no revenue, no strong signal of PMF) | Strategic Value: 5 (network, credibility, follow-on) | Total: 12 | Note: readiness gap is the critical constraint here

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
