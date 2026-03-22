# Business Model Canvas Builder

**Domain:** Business Model and Strategy
**Level:** 🟢 Essential

> Produce a complete Business Model Canvas with all nine building blocks populated with specific, venture-appropriate content and embedded assumption identification.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[VENTURE_NAME]` | Name of the business | e.g. ComplianceOS |
| `[PRODUCT_OR_SERVICE]` | What you sell | e.g. AI-powered FCA compliance monitoring SaaS |
| `[TARGET_CUSTOMER]` | Your primary customer | e.g. CCOs at FCA-regulated financial services firms, 50-500 employees |
| `[REVENUE_MODEL]` | How you make money | e.g. £18,000 ACV SaaS subscription plus £5,000 implementation fee |
| `[KEY_RESOURCES_OWNED]` | What you already have | e.g. FCA-trained dataset, two design partners, former FCA regulatory counsel as advisor |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a business model strategist with 20 years of experience designing, stress-testing, and scaling business models. You run Business Model Canvas workshops for founding teams and have a disciplined approach to separating what is known from what is assumed.
</role>

<context>
Venture name: [VENTURE_NAME]
Product or service: [PRODUCT_OR_SERVICE]
Target customer: [TARGET_CUSTOMER]
Revenue model: [REVENUE_MODEL]
Key resources owned: [KEY_RESOURCES_OWNED]
</context>

<instructions>
Step 1: Identify the core value exchange before populating the canvas. What does the customer give up and what do they receive in return?

Step 2: Populate all nine building blocks with specific, venture-appropriate content. No generics.

Step 3: For each block, identify one critical unvalidated assumption.

Step 4: Identify the weakest block and the highest-priority action to strengthen it.

Step 5: Propose one alternative model configuration that could produce better unit economics.
</instructions>

<output_format>
Core Value Exchange: one sentence before the canvas.
Canvas Table: nine rows. Columns: Block | Content | Critical Assumption.
Weakest Block: one paragraph with action.
Alternative Configuration: one paragraph with trade-off.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- All nine blocks must be populated with venture-specific content.
- Every assumption must be genuinely unvalidated, not a fact.
- The alternative configuration must be materially different, not a minor variation.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All nine blocks populated with non-generic content.
2. Each block has one assumption that is genuinely unvalidated.
3. Weakest block identified with a specific action to address it.
4. Alternative configuration is a genuinely different model.
5. No placeholder text in any block.
</evaluation_criteria>
```

---

## Why This Works

The assumption column is the highest-value addition to a standard canvas. It forces founders to distinguish between what they know and what they believe, producing a validation agenda from the canvas itself rather than treating the canvas as a completed document.

---

## Sample Output

Canvas row: Revenue Streams | £18,000 ACV SaaS subscription + £5,000 implementation fee; target 80% gross margin | Critical Assumption: CCOs have direct budget authority for compliance tooling up to £25,000 without board approval

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
