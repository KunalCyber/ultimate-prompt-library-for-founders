# Build vs Buy vs Partner Decision Framework

**Domain:** Product and Engineering
**Level:** 🔴 Advanced

> Evaluate whether to build, buy, or partner for a specific capability. Produces a structured decision with scoring across cost, speed, control, scalability, and strategic fit.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[CAPABILITY_NEEDED]` | The specific capability you need to add | e.g. Natural language processing to extract compliance obligations from FCA policy documents |
| `[BUILD_OPTION]` | What building in-house would involve | e.g. Hire 1 ML engineer at £80k/year, 4-6 months to first working version, full control, significant ongoing maintenance |
| `[BUY_OPTIONS]` | Available products or APIs you could purchase | e.g. OpenAI GPT-4o API at £0.03 per 1k tokens, AWS Comprehend, or specialist RegTech NLP vendor at £2,000/month |
| `[PARTNER_OPTIONS]` | Potential partners who have this capability | e.g. Partnership with Qdrant (vector DB) plus a prompt engineering consultancy; or white-label agreement with a RegTech data provider |
| `[STRATEGIC_CONTEXT]` | Why this capability matters strategically | e.g. NLP accuracy on FCA documents is our primary differentiator; if a competitor solves this better, we lose our moat |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a technology strategy advisor and CTO coach with 20 years of experience helping founders and engineering leaders make build vs buy vs partner decisions. You understand that this decision has long-term strategic consequences and that the wrong choice is far more expensive than the cost of analysis.
</role>

<context>
Capability needed: [CAPABILITY_NEEDED]
Build option: [BUILD_OPTION]
Buy options: [BUY_OPTIONS]
Partner options: [PARTNER_OPTIONS]
Strategic context: [STRATEGIC_CONTEXT]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Define the evaluation criteria relevant to this specific decision. Consider: Total Cost of Ownership (3-year), Time to First Working Version, Control and Customisability, Scalability, Vendor Risk, and Strategic Differentiation Potential. Weight each criterion based on the stated strategic context.

Step 2: Score each option (Build / each Buy option / each Partner option) across all criteria on a 1-5 scale. Show reasoning for each score.

Step 3: Calculate weighted scores and identify the top two options.

Step 4: Conduct a risk analysis for the top two options. What is the worst-case scenario for each? What is the recovery cost if the wrong choice is made?

Step 5: Produce a clear recommendation with the primary reason and the single most important condition that must be true for the recommendation to hold.
</instructions>

<output_format>
Section 1: Criteria and Weights. Table with Criterion, Weight, and Rationale columns. Weights sum to 100%.
Section 2: Scoring Matrix. Options as columns, criteria as rows. Each cell: score (1-5) with one-phrase rationale. Final row: Weighted Score.
Section 3: Risk Analysis. Two blocks (one per top option): Option, Worst-Case Scenario, Recovery Cost, and Reversibility (Easy/Hard/Irreversible).
Section 4: Recommendation. One decisive paragraph with primary reason and the condition that must hold.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Weights must sum to exactly 100%.
- Scoring must reflect the stated strategic context. If differentiation is the primary concern, the Strategic Differentiation criterion must carry significant weight.
- Risk analysis must be specific to these options, not generic technology risk.
- Recommendation must be unambiguous. No "it depends" conclusions.
- Reversibility assessment must be honest: a custom-built ML model is not easily reversible.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Criteria weights sum to 100%.
2. Strategic differentiation weight reflects the stated strategic context.
3. Weighted scores are mathematically correct.
4. Risk analysis addresses specific worst-case scenarios for each top option.
5. Recommendation names one option with a specific primary reason.
</evaluation_criteria>
```

---

## Why This Works

The reversibility assessment is the most overlooked dimension in build vs buy decisions. A custom-built ML model represents 6-12 months of engineering investment that cannot easily be replaced if it underperforms. Making reversibility explicit forces founders to account for the option value of each path, not just the expected cost.

---

## Sample Output

Risk Analysis: Buy (OpenAI API) | Worst-Case: OpenAI changes pricing by 300% or introduces usage restrictions for regulated financial services use cases, requiring emergency rebuild of the NLP layer | Recovery Cost: 4-6 months of engineering time plus £80k hiring cost | Reversibility: Hard. Switching to a build option after customer contracts are signed on API-dependent pricing is a 6-month disruption.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
