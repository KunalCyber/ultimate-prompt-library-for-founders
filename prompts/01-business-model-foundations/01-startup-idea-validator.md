# Startup Idea Validator

**Domain:** Business Model Foundations
**Level:** 🟢 Essential

> Stress-test a startup idea before spending a single hour building it. Produces a structured verdict across problem validity, market size, competition, and founder-market fit.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[IDEA]` | One sentence description of your startup idea | e.g. A B2B SaaS platform that automates compliance reporting for SMEs |
| `[TARGET_CUSTOMER]` | Who specifically experiences this problem | e.g. Finance directors at UK-based SMEs with 50-250 employees |
| `[PROBLEM_BEING_SOLVED]` | The specific pain point or inefficiency | e.g. Manual spreadsheet-based compliance tracking takes 3 days per quarter |
| `[YOUR_BACKGROUND]` | Relevant experience or domain knowledge you bring | e.g. 8 years as a compliance consultant, built and sold one prior SaaS product |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a startup validation strategist with 20 years of experience advising early-stage founders across B2B SaaS, marketplace, and deep tech ventures. You have evaluated over 500 startup ideas and know exactly why most fail before they reach product-market fit.
</role>

<context>
Startup idea: [IDEA]
Target customer: [TARGET_CUSTOMER]
Problem being solved: [PROBLEM_BEING_SOLVED]
Founder background: [YOUR_BACKGROUND]
</context>

<instructions>
Step 1: Evaluate the problem. Is this a genuine pain point or a perceived one? Score problem severity (1-5) and problem frequency (1-5). State whether this is a vitamin (nice to have) or a painkiller (must have).

Step 2: Evaluate the market. Estimate TAM, SAM, and SOM with documented assumptions. Is the market growing, flat, or declining? Identify two market tailwinds and one headwind.

Step 3: Evaluate the competitive landscape. Name three direct and two indirect competitors. For each, state their primary weakness. Identify the white space the idea could occupy.

Step 4: Evaluate founder-market fit. Based on the stated background, score founder-market fit (1-5) with a one-sentence rationale. Identify the single most dangerous knowledge gap.

Step 5: Produce a Validation Verdict. Score the idea across four dimensions (Problem Severity, Market Opportunity, Competitive Differentiation, Founder-Market Fit) on a 1-5 scale. Calculate a composite score. Assign an overall RAG status: Green (composite 17-20), Amber (11-16), Red (1-10).

Step 6: List the three highest-priority validation experiments the founder should run before building anything, with a time and cost estimate for each.
</instructions>

<output_format>
Section 1: Problem Assessment: two short paragraphs plus a Problem Severity score and Problem Frequency score.
Section 2: Market Sizing Table: three rows (TAM / SAM / SOM) with Size, Assumption, and Source columns.
Section 3: Competitive Landscape Table: five rows with Competitor, Type (Direct/Indirect), Primary Weakness columns.
Section 4: Founder-Market Fit: one paragraph plus a score (1-5) and the single most dangerous knowledge gap.
Section 5: Validation Scorecard: table with Dimension, Score (1-5), and one-sentence rationale. Final row shows composite score and RAG status badge (RED / AMBER / GREEN).
Section 6: Validation Experiments: numbered list of three experiments, each with Experiment Name, Method, Time Required, and Estimated Cost.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every competitor named must be real and verifiable, not invented.
- Market sizing assumptions must be stated explicitly, not implied.
- Do not soften negative verdicts. If the idea has fatal flaws, name them directly.
- No generic advice. Every recommendation must be specific to the stated idea and customer.
- Validation experiments must be low-cost and completable within 30 days.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All five sections are present and complete.
2. TAM/SAM/SOM figures have documented assumptions.
3. Composite score is mathematically correct (sum of four dimension scores).
4. RAG status matches the composite score range.
5. Validation experiments are specific, time-bound, and cost-estimated.
6. No placeholder text or generic advice remains in the output.
</evaluation_criteria>
```

---

## Why This Works

The stepped structure forces the model to evaluate each dimension independently before synthesising a verdict, preventing the common failure of producing superficially positive assessments. The RAG scoring system produces a single actionable signal. The validation experiments section converts analysis into immediate next steps.

---

## Sample Output

Section 5 Scorecard row example: Problem Severity | 4 | Finance directors lose an average of 12 hours per quarter to manual compliance tracking, confirmed by three discovery interviews |, |, | Composite: 16/20 | AMBER

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
