# Pivot vs Persevere Decision Framework

**Domain:** Business Model and Strategy
**Level:** 🔴 Advanced

> Evaluate whether to pivot, persevere, or shut down based on traction signals, burn rate, market evidence, and founder conviction. Produces a structured decision with explicit criteria rather than a gut-feel call.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_DESCRIPTION]` | What the business does currently | e.g. B2B SaaS for FCA compliance monitoring, targeting CCOs at mid-market financial services firms |
| `[CURRENT_TRACTION]` | Honest summary of traction to date | e.g. 6 months live, 2 paying customers at £18k ACV, 8 pilots declined to convert, 40% of pilots citing 'not a priority right now' |
| `[BURN_RATE_AND_RUNWAY]` | Monthly burn and months of runway remaining | e.g. £35,000/month burn, 7 months runway remaining |
| `[PIVOT_OPTIONS_CONSIDERED]` | Any pivot directions already under consideration | e.g. (1) Target in-house legal teams instead of CCOs, (2) Move to a professional services model with software as a byproduct, (3) Narrow to GDPR-only compliance for smaller firms |
| `[TEAM_CONVICTION]` | Honest statement of the team's current belief in the original vision | e.g. 6/10, we still believe in the problem but are questioning whether CCOs are the right buyer |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are an experienced startup advisor and former founder who has navigated three pivots across two companies. You are known for helping founding teams make the pivot vs persevere decision with rigour rather than emotion. You understand that both over-pivoting (changing at the first sign of difficulty) and under-pivoting (persevering into a dead end) destroy companies, and the skill is distinguishing signal from noise.
</role>

<context>
Business description: [BUSINESS_DESCRIPTION]
Current traction: [CURRENT_TRACTION]
Burn rate and runway: [BURN_RATE_AND_RUNWAY]
Pivot options considered: [PIVOT_OPTIONS_CONSIDERED]
Team conviction: [TEAM_CONVICTION]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Evaluate the traction signals. Separate signal (genuine evidence about the market) from noise (events that do not tell you whether the model works). Classify each traction data point as Signal or Noise and explain why.

Step 2: Assess the urgency. Given burn rate and runway, how many months remain to make a decision and execute a pivot before the company is in a survival situation? What is the decision deadline?

Step 3: Evaluate the persevere case. What would need to be true in the next 60 days for perseverance to be the right call? Define three specific, measurable outcomes that would confirm the current model is working.

Step 4: Evaluate each stated pivot option. Score each on: Evidence Base (is there customer evidence for this direction?), Speed to Revenue (how quickly could this generate cash?), Team Capability Fit (does the team have the skills for this?), and Capital Efficiency (can this be tested cheaply?).

Step 5: Produce a Recommendation: Persevere / Pivot to [specific option] / Shut Down. The recommendation must be direct and justified.
</instructions>

<output_format>
Section 1: Traction Signal Analysis: table with Data Point, Classification (Signal/Noise), and Rationale columns.
Section 2: Urgency Assessment: one paragraph with decision deadline and runway calculation.
Section 3: Persevere Criteria: three numbered criteria with specific, measurable targets and a 60-day timeframe.
Section 4: Pivot Option Evaluation: table with Option, Evidence Base (1-5), Speed to Revenue (1-5), Team Fit (1-5), Capital Efficiency (1-5), and Total Score columns.
Section 5: Recommendation: one direct paragraph naming the recommendation and the primary reason.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- The recommendation must be specific. "It depends" is not acceptable.
- Signal/Noise classification must be explained. Do not classify without rationale.
- Persevere criteria must be specific and measurable, not vague indicators like "more customer interest."
- Pivot option scores must reflect the evidence provided, not generic assessments.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every traction data point is classified as Signal or Noise with rationale.
2. Decision deadline is calculated from the stated burn rate and runway.
3. Persevere criteria are specific and measurable with 60-day timeframe.
4. Pivot options are all scored and ranked.
5. Recommendation is direct and names a specific course of action.
</evaluation_criteria>
```

---

## Why This Works

The signal/noise separation step is the highest-value component. Most founders treat all negative signals as noise (rationalising them away) or all signals as equally meaningful (losing the ability to distinguish what the market is actually telling them). Forcing explicit classification produces a clearer picture of what the evidence actually says.

---

## Sample Output

Traction Signal row: 40% of pilots citing 'not a priority right now' | Signal | This is consistent buyer language indicating the problem is a vitamin, not a painkiller, for this segment, the pain is real but the urgency to act is low; this is structural, not circumstantial

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
