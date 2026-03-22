# Beachhead Market Selector

**Domain:** Business Model Foundations
**Level:** 🔴 Advanced

> Analyse multiple market segments and select the optimal beachhead market based on size, accessibility, willingness to pay, expansion potential, and competitive intensity. Prevents the fatal error of targeting everyone.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you are selling | e.g. AI-powered legal document review platform |
| `[CANDIDATE_SEGMENTS]` | List 3-5 market segments you are considering targeting first | e.g. (1) Magic Circle law firms, (2) Regional UK law firms 20-100 lawyers, (3) In-house legal teams at FTSE 250 companies, (4) Legal aid providers, (5) LegalTech consultancies |
| `[YOUR_CONSTRAINTS]` | Budget, team size, and time horizon for gaining traction | e.g. £200k runway, 2-person team, need first paying customer within 6 months |
| `[CORE_CAPABILITY]` | The single strongest capability or advantage your product has | e.g. Processes UK contract law nuance with 94% accuracy vs 71% for US-trained models |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a go-to-market strategist with 20 years of experience helping B2B companies select and dominate beachhead markets before expanding. You have advised companies from Series A through IPO on market entry sequencing. You understand that the beachhead market decision is often the most important strategic choice an early-stage company makes.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Candidate segments: [CANDIDATE_SEGMENTS]
Constraints: [YOUR_CONSTRAINTS]
Core capability: [CORE_CAPABILITY]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Define the evaluation criteria relevant to beachhead market selection: (a) Segment size and reachability, (b) Urgency of the problem, (c) Willingness to pay, (d) Sales cycle length, (e) Competitive intensity, (f) Expansion potential to adjacent segments, (g) Alignment with core capability. Weight each criterion.

Step 2: Score each candidate segment against each criterion on a 1-5 scale. Show your reasoning for each score briefly.

Step 3: Calculate weighted scores for each segment. Identify the top two segments.

Step 4: For the top two segments, conduct a head-to-head comparison. Identify the tie-breaker factor given the stated constraints.

Step 5: Recommend the beachhead market with a clear rationale. Identify the single most important action to take in the first 30 days to establish presence in that segment.
</instructions>

<output_format>
Section 1: Evaluation Criteria: table with Criterion, Weight (must sum to 100%), and Rationale for Weight columns.
Section 2: Segment Scoring Matrix: table with segments as columns and criteria as rows. Each cell contains a score (1-5) with a one-phrase rationale. Final row: Weighted Score per segment.
Section 3: Head-to-Head Comparison: structured comparison of the top two segments across five dimensions relevant to the stated constraints.
Section 4: Beachhead Recommendation: one decisive paragraph naming the recommended segment, the primary reason, and the single most important 30-day action.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Weights must sum to exactly 100%.
- Weighted scores must be mathematically correct.
- The recommendation must be specific and unambiguous. Do not recommend "either could work."
- The 30-day action must be specific and actionable, not generic advice like "talk to customers."
- Scores must reflect genuine differentiation between segments. Avoid clustering all segments at 3/5.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Criterion weights sum to exactly 100%.
2. Weighted scores are mathematically correct for each segment.
3. Head-to-head comparison addresses the stated constraints specifically.
4. Recommendation names one segment clearly with no hedging.
5. 30-day action is specific and immediately actionable.
</evaluation_criteria>
```

---

## Why This Works

The weighted scoring matrix prevents founders from selecting a beachhead based on familiarity or enthusiasm rather than strategic logic. The explicit weighting step forces a decision about what matters most given the stated constraints, making the scoring criteria reflect the actual situation rather than generic best practice.

---

## Sample Output

Segment Scoring row: Willingness to Pay (Weight: 20%) | Magic Circle: 3, high WTP but long procurement cycles | Regional firms: 4, budget-holder is accessible, faster decision | In-house: 2, procurement requires legal ops sign-off and IT security review

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
