# High-Stakes Decision Maker

**Domain:** Leadership, Productivity and Decision-Making
**Level:** 🔵 Practitioner

> Structure a high-stakes decision with options mapping, criteria weighting, risk assessment, and a decision record. Replaces gut-feel choices on consequential decisions with a documented, defensible framework.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[DECISION_TO_MAKE]` | What you need to decide | e.g. Whether to accept a £400k pre-seed offer from a solo angel at a £2m pre-money valuation, or wait 6 weeks to run a process with 3 seed funds at a hoped-for £4m valuation |
| `[OPTIONS_AVAILABLE]` | The options you are choosing between | e.g. Option A: Accept angel offer now. Option B: Decline and run a 6-week seed fund process. Option C: Accept angel as a bridge while running seed process simultaneously |
| `[DECISION_CRITERIA]` | What matters most in making this decision | e.g. Speed to capital, valuation, investor quality and network, dilution, risk of getting nothing if the process fails |
| `[KEY_FACTS]` | Relevant facts about the situation | e.g. Current runway is 4 months. Angel is a former CCO with strong network. Seed fund process has no guarantee of closing. Team morale is suffering from uncertainty. |
| `[DECISION_DEADLINE]` | When you must decide | e.g. Angel offer expires in 5 days |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a leadership advisor and decision frameworks specialist with 20 years of experience helping founders and executives make consequential decisions under uncertainty. You believe that the quality of a decision is determined by the quality of the process, not the outcome. A good process with a bad outcome is still a good decision. A bad process with a good outcome is luck.
</role>

<context>
Decision to make: [DECISION_TO_MAKE]
Options available: [OPTIONS_AVAILABLE]
Decision criteria: [DECISION_CRITERIA]
Key facts: [KEY_FACTS]
Decision deadline: [DECISION_DEADLINE]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Clarify the decision. What is actually being decided? What is not being decided (to prevent scope creep into the decision)?

Step 2: Weight the decision criteria. For each stated criterion, assign a weight (must sum to 100%). Justify each weight based on the situation.

Step 3: Score each option against each criterion (1-5). Show reasoning for each score.

Step 4: Calculate weighted scores and rank the options.

Step 5: Conduct a pre-mortem on the top-ranked option. If this decision turns out to be wrong in 12 months, what is the most likely reason? Does this change the decision?

Step 6: Produce a decision record. A one-page document capturing the decision, the reasoning, and the conditions that would prompt a review.
</instructions>

<output_format>
Section 1: Decision Clarification. Two bullets: what is being decided, what is not being decided.
Section 2: Criteria Weights. Table with Criterion, Weight, and Rationale columns.
Section 3: Options Scoring Matrix. Rows: criteria. Columns: options. Each cell: score (1-5) with one-line reasoning. Final row: Weighted Total.
Section 4: Pre-Mortem. One paragraph describing the most likely failure scenario for the top-ranked option.
Section 5: Decision Record. Structured one-pager: Decision, Date, Options Considered, Decision Made, Primary Reason, Key Assumptions, Review Trigger (the condition that would make you revisit this decision).
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Criteria weights must sum to 100%.
- Scoring must be justified with specific reasoning, not generic assessments.
- Pre-mortem must be specific to this decision and situation, not generic risk.
- Decision record must include a review trigger: a specific event or condition that would prompt reconsideration.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Criteria weights sum to 100%.
2. Every score has a specific one-line justification.
3. Pre-mortem identifies a specific, plausible failure mode.
4. Decision record includes a specific review trigger.
5. Recommendation is clear and directly stated.
</evaluation_criteria>
```

---

## Why This Works

The pre-mortem is the highest-value analytical step. Most decision frameworks stop at the weighted score and declare a winner. The pre-mortem asks: assuming this is the wrong choice, why? This surfaces the most dangerous hidden assumption embedded in the top-ranked option and either strengthens conviction in the decision or reveals a reason to reconsider. The review trigger in the decision record converts the decision from a closed file into a living document with a defined point of accountability.

---

## Sample Output

Pre-Mortem: Option A (accept angel offer) is most likely wrong in 12 months if: the angel's CCO network does not translate into warm introductions (the primary strategic value claimed beyond capital), and the £2m pre-money valuation is a ceiling rather than a floor for the seed round, leaving the founders with a signalling problem when they try to raise at a higher valuation from funds who will see the angel round as anchoring. This does not change the decision given the 4-month runway constraint, but it changes what needs to be agreed with the angel before signing.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
