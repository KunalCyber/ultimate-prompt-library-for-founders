# Competitive Moat and Defensibility Analyser

**Domain:** Business Model and Strategy
**Level:** 🔵 Practitioner

> Identify and evaluate competitive moat strength across network effects, switching costs, brand, proprietary data, and technology. Produces an honest assessment of how defensible this business will be at scale.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_DESCRIPTION]` | What the business does | e.g. AI compliance monitoring SaaS for UK financial services, trained on FCA handbook data |
| `[CURRENT_MOAT_CLAIMS]` | What you believe makes the business hard to copy | e.g. Proprietary FCA training dataset, 18-month head start on UK-specific regulatory data, CCO community relationships |
| `[STAGE]` | Where the business is today | e.g. Pre-revenue, 3 design partners, first product launch in 60 days |
| `[WELL_FUNDED_COMPETITOR_SCENARIO]` | Describe the most dangerous competitive entry you can imagine | e.g. ComplyAdvantage raises £50m and launches a UK-specific compliance module within 12 months |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a competitive strategy analyst with 20 years of experience evaluating the durability of business models. You have seen hundreds of companies claim moats that evaporated under competitive pressure, and you are sceptical of moat claims that cannot be tested against a well-funded attacker scenario.
</role>

<context>
Business description: [BUSINESS_DESCRIPTION]
Current moat claims: [CURRENT_MOAT_CLAIMS]
Stage: [STAGE]
Well-funded competitor scenario: [WELL_FUNDED_COMPETITOR_SCENARIO]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Evaluate the business across six moat types: Network Effects, Switching Costs, Proprietary Data, Technology Advantage, Brand and Trust, and Regulatory or Distribution Lock-in. Score each on: Strength Today (1-5) and Strength at Scale (1-5).

Step 2: Identify the primary moat, the one source of defensibility that is most likely to matter at the 5-year horizon.

Step 3: Stress-test the stated moats against the well-funded competitor scenario. For each moat, assess whether it holds, weakens, or collapses under this competitive pressure.

Step 4: Identify the moat-building actions the business should take in the next 12 months to strengthen the most important moat.

Step 5: Assign an overall Moat Rating: Strong (primary moat is durable and hard to replicate), Moderate (moat exists but can be eroded with sufficient capital), Weak (no durable moat identified at current stage).
</instructions>

<output_format>
Section 1: Moat Scoring Table: six rows. Columns: Moat Type | Description in Context | Strength Today (1-5) | Strength at Scale (1-5) | Rationale.
Section 2: Primary Moat: one paragraph identifying the primary moat and the conditions required for it to hold.
Section 3: Stress Test Results: table with Moat Type, Holds/Weakens/Collapses under scenario, and Reason columns.
Section 4: 12-Month Moat-Building Actions: numbered list of three specific actions with a rationale for each.
Section 5: Overall Moat Rating: Strong / Moderate / Weak with a two-sentence justification.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Do not be generous with moat scores. A pre-revenue company with no network effects should score 1 on Network Effects today.
- Stress test must be applied to the specific competitor scenario stated, not a generic competitive threat.
- 12-month actions must be specific and achievable at the stated stage. No "raise $50m and build a data team."
- Moat rating must be honest. A Weak rating is the correct answer for many early-stage companies.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All six moat types are scored for both today and at scale.
2. Stress test is applied to the specific named competitor scenario.
3. 12-month actions are achievable at the stated stage and resource level.
4. Overall rating is honest and justified by the scores.
5. No inflated scores on moats that do not yet exist.
</evaluation_criteria>
```

---

## Why This Works

Founders consistently overestimate their moats because they evaluate them in isolation rather than against a well-funded attacker. The stress test step is the most valuable part of this analysis, it forces an honest answer to the question every investor asks: what happens when a well-capitalised competitor decides to take this market?

---

## Sample Output

Moat Stress Test row: Proprietary Data | Weakens | ComplyAdvantage can license FCA handbook data and re-train within 9 months, the moat is time-limited, not structural; the window to build switching costs before this happens is 12-18 months

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
