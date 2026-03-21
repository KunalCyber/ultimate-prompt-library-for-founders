# Ideal Customer Profile and Persona Builder

**Domain:** Go-to-Market and Launch
**Level:** 🔵 Practitioner

> Define your ICP with demographic, firmographic, psychographic, behavioural, and pain-point detail. Produces a working ICP document that your sales and marketing teams can actually use.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you sell | e.g. AI compliance monitoring SaaS for UK financial services |
| `[CURRENT_BEST_CUSTOMERS]` | Describe your best existing customers or design partners if you have them | e.g. CCO at a 150-person FCA-regulated investment manager; personally handles compliance reporting; 12 years in compliance; has tried two prior tools that failed due to UK regulatory gaps |
| `[PROBLEM_YOU_SOLVE]` | The specific problem and the cost of not solving it | e.g. Quarterly FCA compliance reporting takes 3 days of manual work; one missed obligation can trigger an FCA fine averaging £250k |
| `[REVENUE_MODEL]` | How you charge | e.g. £18,000 ACV SaaS, annual contract, direct sale to CCO |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a go-to-market strategist and ICP specialist with 15 years of experience defining and refining ideal customer profiles for B2B SaaS companies from pre-revenue through Series B. You understand that an ICP is not a demographic description: it is a precise definition of the customer who has the most urgent problem, the highest willingness to pay, the shortest sales cycle, and the greatest expansion potential.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Current best customers: [CURRENT_BEST_CUSTOMERS]
Problem you solve: [PROBLEM_YOU_SOLVE]
Revenue model: [REVENUE_MODEL]
</context>

<instructions>
Step 1: Define the ICP at firmographic level. What company size, industry, geography, regulatory environment, and growth stage characterises the ideal customer organisation?

Step 2: Define the ICP at buyer level. Who is the economic buyer, the technical buyer, and the champion? For each, define: role, seniority, primary motivation, primary fear, and how they typically make this type of decision.

Step 3: Define the trigger events. What specific events or circumstances cause an ideal customer to actively seek a solution right now? These are the moments to intercept.

Step 4: Define the disqualification criteria. What characteristics should immediately remove a prospect from the pipeline? Being specific about who you will not sell to is as important as defining who you will.

Step 5: Produce a one-page ICP summary card suitable for use by a sales or marketing team without you present to explain it.
</instructions>

<output_format>
Section 1: Firmographic ICP. Table with Dimension and Ideal Profile columns. Dimensions: Company Size, Industry, Geography, Regulatory Environment, Tech Stack Maturity, Growth Stage.
Section 2: Buyer Personas. Three persona blocks (Economic Buyer, Technical Buyer, Champion). Each: Role, Seniority, Primary Motivation, Primary Fear, Decision Style.
Section 3: Trigger Events. Numbered list of five specific trigger events with a one-sentence description of why each creates urgency.
Section 4: Disqualification Criteria. Numbered list of five disqualifiers with the reason for disqualification.
Section 5: ICP Summary Card. Formatted as a concise reference document: one paragraph on ideal company, one paragraph on ideal buyer, three trigger events, three disqualifiers.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Trigger events must be specific and observable, not vague conditions like "when they are growing."
- Disqualification criteria must be specific enough to apply in a 10-minute discovery call.
- Buyer personas must reflect real decision dynamics, not org chart logic.
- The ICP summary card must be usable without explanation or context.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All six firmographic dimensions are defined with specific criteria.
2. Three distinct buyer roles are profiled with different motivations and fears.
3. Trigger events are specific and observable.
4. Disqualification criteria are specific enough to apply in discovery.
5. ICP summary card is self-contained and usable without the full document.
</evaluation_criteria>
```

---

## Why This Works

The trigger event identification is the highest-value ICP component most companies skip. Knowing who your ideal customer is tells you who to target. Knowing when they are actively buying tells you when to reach them. The disqualification criteria are equally important: most B2B sales failures are not lost deals but deals that should never have entered the pipeline.

---

## Sample Output

Trigger Event 3: FCA regulatory change published. When the FCA publishes a PS (Policy Statement) or CP (Consultation Paper) that creates new compliance obligations, CCOs face a 6-12 month implementation window. This is the highest-urgency buying moment: the problem is explicit, the deadline is published, and the budget is typically pre-approved as part of regulatory change management.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
