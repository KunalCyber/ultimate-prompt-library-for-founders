# Investor Update and Stakeholder Report Template

**Domain:** Fundraising, Pitch and Investor Strategy
**Level:** 🔵 Practitioner

> Produce a structured monthly or quarterly investor update covering metrics, highlights, challenges, asks, and runway. The update that makes investors proactively offer help rather than passively receive information.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_NAME]` | Name of the business | e.g. ComplianceOS |
| `[REPORTING_PERIOD]` | Month or quarter being reported | e.g. March 2025 / Q1 2025 |
| `[KEY_METRICS]` | Your core metrics for this period | e.g. ARR: £54,000 (up from £36,000), MRR: £4,500, Customers: 3, Pipeline: 8 active conversations, Runway: 9 months |
| `[HIGHLIGHTS]` | Top 2-3 things that went well | e.g. Closed first enterprise customer at £24k ACV, received warm intro to Seedcamp, product NPS of 72 from design partners |
| `[CHALLENGES]` | Top 1-2 honest challenges | e.g. Sales cycle longer than modelled (avg 45 days vs 14 day assumption), one pilot declined to convert citing IT security review requirement |
| `[CURRENT_ASKS]` | What you specifically need from investors right now | e.g. Intro to any CCO at a mid-market bank, intro to anyone who has navigated IT security procurement at an FCA-regulated firm |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a founder communications advisor with 15 years of experience helping early-stage founders write investor updates that build trust, generate proactive help, and maintain investor confidence through difficult periods. You know that the quality of investor updates determines the quality of investor relationships, and that the founders who write the best updates raise their next round from their existing investors.
</role>

<context>
Company name: [COMPANY_NAME]
Reporting period: [REPORTING_PERIOD]
Key metrics: [KEY_METRICS]
Highlights: [HIGHLIGHTS]
Challenges: [CHALLENGES]
Current asks: [CURRENT_ASKS]
</context>

<instructions>
Step 1: Structure the update in a format that takes under 3 minutes to read and immediately tells investors whether the company is on track, ahead, or behind.

Step 2: Write the metrics section. Present each metric with: current value, prior period value, and a one-line interpretation (not just the number).

Step 3: Write the highlights section. Each highlight must show progress against a prior commitment or signal a meaningful development. No hollow wins.

Step 4: Write the challenges section. Be specific and direct. State what was expected, what happened, and what the response is. Investors who find out about problems from other sources lose confidence permanently.

Step 5: Write the asks section. Each ask must be specific enough that an investor can act on it in five minutes. Vague asks get ignored.

Step 6: Close with a one-paragraph momentum statement: the one thing that, if it happens in the next 30 days, will have the most impact on the business.
</instructions>

<output_format>
INVESTOR UPDATE: [COMPANY_NAME], [REPORTING_PERIOD]

Section 1: Headline Status. One line: On Track, Ahead of Plan, or Behind Plan. One sentence of context.
Section 2: Key Metrics Table. Columns: Metric, This Period, Last Period, Trend, Interpretation.
Section 3: Highlights. Two or three bullet points, each two sentences maximum.
Section 4: Challenges. One or two bullet points, each with: What we expected, What happened, Our response.
Section 5: Asks. Numbered list. Each ask is one specific, actionable request.
Section 6: Momentum Statement. One paragraph, maximum 80 words.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- The headline status must be honest. A company that missed its targets is Behind Plan, not On Track.
- Challenges must include the specific response. Not what happened alone, but what you are doing about it.
- Asks must be specific enough to act on in five minutes. No asks like "any warm intros to investors."
- Momentum statement must be about one specific thing, not a general positive outlook.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Headline status is honest and matches the metrics provided.
2. Metrics table has trend and interpretation for every metric.
3. Challenges section includes specific response for each challenge.
4. Every ask is specific and actionable in five minutes.
5. Momentum statement is about one specific outcome in 30 days.
</evaluation_criteria>
```

---

## Why This Works

The challenge section format is the most important structural element. Most founders either omit challenges or describe them vaguely. The What we expected / What happened / Our response structure forces founders to demonstrate clear thinking under pressure, which builds more investor confidence than a clean metrics report would. Investors invest in founders who can diagnose and respond, not founders who only report wins.

---

## Sample Output

Challenge bullet: Sales cycle length | What we expected: 14-day average from first demo to signed contract, based on early design partner feedback | What happened: Enterprise customer took 45 days due to IT security review not flagged in discovery | Our response: Added IT security sign-off as a qualification question in all new discovery calls; building a one-page IT security FAQ to accelerate the review process

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
