# One-Page Business Clarity Document

**Domain:** Business Model Foundations
**Level:** 🟢 Essential

> Produce a single, structured one-page document that forces complete clarity on what the business does, who it serves, how it makes money, what makes it different, and where it is going. The document a founder should be able to hand to any investor, partner, or hire.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_NAME]` | Name of the business | e.g. ComplianceOS |
| `[WHAT_YOU_DO]` | One sentence description of the product or service | e.g. Automates FCA compliance evidence collection for regulated financial services firms |
| `[WHO_YOU_SERVE]` | Specific customer description | e.g. Chief Compliance Officers at UK-regulated financial services firms with 100-500 employees |
| `[HOW_YOU_MAKE_MONEY]` | Revenue model with specifics | e.g. Annual SaaS subscription at £18,000 per firm, implementation fee of £5,000 |
| `[WHAT_MAKES_YOU_DIFFERENT]` | Specific differentiation, not generic claims | e.g. Only platform trained on FCA handbook, US competitors produce 30% error rate on UK-specific obligations |
| `[WHERE_YOU_ARE_GOING]` | 12-month goal | e.g. 10 paying customers, £180k ARR, Series A ready |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a business clarity consultant who has worked with over 300 founding teams to cut through complexity and produce precise, compelling articulations of their business. You believe that if a founder cannot explain their business in one page with complete specificity, they do not yet understand it well enough to scale it.
</role>

<context>
Business name: [BUSINESS_NAME]
What you do: [WHAT_YOU_DO]
Who you serve: [WHO_YOU_SERVE]
How you make money: [HOW_YOU_MAKE_MONEY]
What makes you different: [WHAT_MAKES_YOU_DIFFERENT]
Where you are going: [WHERE_YOU_ARE_GOING]
</context>

<instructions>
Step 1: Review the inputs for consistency. Flag any contradictions or gaps before producing the document.

Step 2: Produce the One-Page Business Clarity Document with six sections. Each section must be sharp, specific, and free of filler language.

Step 3: Score the clarity of each section (1-5) based on specificity, memorability, and absence of generic language. Identify the section that needs the most work and explain why.

Step 4: Produce one alternative phrasing for the single weakest section that materially improves its clarity or impact.
</instructions>

<output_format>
ONE-PAGE BUSINESS CLARITY DOCUMENT, [BUSINESS_NAME]

1. WHAT WE DO
[One sentence, active voice, specific outcome delivered to specific customer]

2. WHO WE SERVE
[One sentence with three specificity layers: role, company type, and defining characteristic]

3. THE PROBLEM WE SOLVE
[Two sentences: the current state without the product, and the cost of that current state]

4. HOW WE MAKE MONEY
[One sentence: pricing model, price point, and contract structure]

5. WHAT MAKES US DIFFERENT
[Two sentences: the specific, verifiable claim that differentiates this product from alternatives]

6. WHERE WE ARE GOING
[One sentence: 12-month goal expressed as measurable outcome]

---
Clarity Scores: table with Section, Score (1-5), and one-line rationale.
Weakest Section Improvement: the original line, followed by the alternative.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- No marketing language. No claims that cannot be verified or substantiated.
- No generic differentiation claims such as "we are more user-friendly" or "we have better customer service."
- Every section must be one or two sentences maximum.
- If an input is vague or generic, flag it in the consistency check before attempting to improve it.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. The document is precisely one page when formatted at normal reading size.
2. Every section is one or two sentences maximum.
3. The differentiation claim is specific and verifiable, not generic.
4. Clarity scores are honest. If a section is weak, score it accordingly.
5. The alternative phrasing for the weakest section is materially better, not a minor word swap.
</evaluation_criteria>
```

---

## Why This Works

The scoring layer prevents the common failure of producing a one-pager that looks complete but is filled with vague claims. Forcing a score on each section and then improving the weakest one ensures the document does not just exist but is genuinely sharp. The consistency check step catches contradictions that would undermine investor confidence.

---

## Sample Output

Clarity Score row: What Makes Us Different | 2 | Current phrasing uses 'best-in-class' without a verifiable claim, needs a specific, evidenced differentiator | Alternative: 'The only FCA-trained compliance platform: UK law firm clients report 94% accuracy vs 71% for US-trained alternatives in independent testing'

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
