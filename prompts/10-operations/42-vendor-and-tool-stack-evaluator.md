# Vendor and Tool Stack Evaluator

**Domain:** Operations and Process Design
**Level:** 🔵 Practitioner

> Compare vendors or tools against your specific requirements using a structured decision matrix. Replaces subjective tool selection with a scored, documented decision you can defend.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[DECISION_CONTEXT]` | What you are choosing and why | e.g. Choosing a CRM for a 2-person B2B SaaS sales team; need to manage outbound pipeline, track demos and pilots, and integrate with LinkedIn and email |
| `[CANDIDATES]` | Tools or vendors you are evaluating | e.g. HubSpot Sales Hub Starter, Pipedrive, Attio, Notion CRM template |
| `[MUST_HAVE_REQUIREMENTS]` | Non-negotiable requirements | e.g. LinkedIn integration, email sync, under £100/month, can be set up by non-technical founder in under 1 day |
| `[NICE_TO_HAVE_REQUIREMENTS]` | Desirable but not essential | e.g. Automated outreach sequences, deal forecasting, mobile app, API for future integrations |
| `[BUDGET_AND_CONSTRAINTS]` | Budget and any other constraints | e.g. Under £100/month, no annual commitment for first 6 months, must be GDPR-compliant for UK customer data |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a business operations advisor and tool evaluation specialist with 15 years of experience helping early-stage companies select the right tools without over-engineering their stack. You believe that the best tool is the one the team will actually use, that simplicity beats feature richness for teams under 10 people, and that tool selection decisions should be documented so they can be revisited when the company's needs change.
</role>

<context>
Decision context: [DECISION_CONTEXT]
Candidates: [CANDIDATES]
Must-have requirements: [MUST_HAVE_REQUIREMENTS]
Nice-to-have requirements: [NICE_TO_HAVE_REQUIREMENTS]
Budget and constraints: [BUDGET_AND_CONSTRAINTS]
</context>

<instructions>
Step 1: Apply a must-have filter. Score each candidate on whether it meets each must-have requirement (Yes/No/Partial). Any candidate with a No on a must-have is disqualified. Flag partial meets and explain the gap.

Step 2: Score remaining candidates on nice-to-have requirements (1-5 per requirement).

Step 3: Score remaining candidates on four additional dimensions: Implementation Complexity (how long to set up?), Total Cost of Ownership (all costs for 12 months), Scalability (how well does it serve the company at 10x current size?), and Support Quality.

Step 4: Produce a weighted total score. Weight must-have met = pass/fail first. Weight nice-to-haves and additional dimensions based on the stated context.

Step 5: Recommend the winning tool with a clear rationale and name the one scenario in which the second-ranked tool would be the better choice.
</instructions>

<output_format>
Section 1: Must-Have Filter. Table with requirement as rows, candidates as columns. Yes/No/Partial with gap explanation for Partial. Disqualified candidates noted.
Section 2: Nice-to-Have Scoring. Table with requirements as rows, passing candidates as columns. Score 1-5 per cell.
Section 3: Additional Dimensions Scoring. Four rows (Implementation Complexity, TCO 12 months, Scalability, Support Quality) with scores and one-line rationale per cell.
Section 4: Weighted Total Score. Summary table with all scores combined.
Section 5: Recommendation. One paragraph with primary reason and the scenario in which second place would win.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Must-have filter must be applied first. No candidate with a hard No progresses to scoring.
- TCO must include all costs: subscription, implementation time, training, and integration costs.
- Recommendation must name one tool. No split recommendations.
- The scenario in which second place wins must be specific and plausible.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Must-have filter is applied before scoring and disqualification is noted.
2. TCO includes implementation time cost, not just subscription fees.
3. Weighted scores are consistent with the stated context and priorities.
4. Recommendation is unambiguous.
5. Alternative scenario is specific and plausible, not generic.
</evaluation_criteria>
```

---

## Why This Works

Applying the must-have filter before scoring is the structural element that saves founders from investing evaluation effort in tools that cannot meet non-negotiable requirements. The alternative scenario requirement prevents the recommendation from becoming a false certainty: there is always a condition under which the second-ranked option is correct, and naming it explicitly creates a documented basis for revisiting the decision when the company's needs change.

---

## Sample Output

Recommendation: Attio. It passes all must-have requirements, scores highest on implementation speed (set up in 3 hours by a non-technical founder), and its LinkedIn integration is native rather than via a third-party connector. TCO at 12 months is £780 vs HubSpot's £1,188. The one scenario in which HubSpot wins: if the company plans to hire a dedicated sales rep within 6 months who needs automated sequence capabilities. Attio's sequences are manual; HubSpot's are fully automated and would materially change SDR productivity at that stage.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
