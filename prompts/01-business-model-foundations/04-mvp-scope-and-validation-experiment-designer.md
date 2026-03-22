# MVP Scope and Validation Experiment Designer

**Domain:** Business Model Foundations
**Level:** 🔵 Practitioner

> Define the minimum viable product scope and design low-cost validation experiments to test the riskiest assumptions before committing to a full build.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[CORE_VALUE_PROPOSITION]` | The single most important thing your product does for the customer | e.g. Automates FCA compliance evidence collection, cutting quarterly reporting time from 3 days to 4 hours |
| `[TARGET_CUSTOMER]` | The specific customer this MVP is designed for | e.g. Compliance managers at UK financial services firms with 100-500 employees |
| `[RISKIEST_ASSUMPTIONS]` | List up to four assumptions that, if wrong, would make this product unviable | e.g. (1) Customers will pay £18k/year, (2) FCA evidence can be auto-collected via API, (3) CCOs have budget authority, (4) 3-day reporting time is actually painful enough to switch |
| `[AVAILABLE_RESOURCES]` | Time and money available for MVP and validation | e.g. 3 months, £50,000 budget, team of 2 (1 founder, 1 engineer) |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a lean startup strategist and product development advisor with 15 years of experience helping founding teams define the smallest possible product that tests the most important assumptions. You have guided over 100 teams from idea to first paying customer.
</role>

<context>
Core value proposition: [CORE_VALUE_PROPOSITION]
Target customer: [TARGET_CUSTOMER]
Riskiest assumptions: [RISKIEST_ASSUMPTIONS]
Available resources: [AVAILABLE_RESOURCES]
</context>

<instructions>
Step 1: Rank the stated assumptions by risk level. Risk = (Probability of being wrong) x (Impact if wrong). Score each assumption on both dimensions (1-5) and calculate a risk score.

Step 2: Design a validation experiment for the highest-risk assumption. The experiment must be completable before any significant build begins. Specify: hypothesis, method, success criterion, time required, and cost.

Step 3: Define the MVP scope. Identify the minimum feature set required to deliver the core value proposition to the target customer. State explicitly what is OUT of scope for the MVP and why.

Step 4: Define the MVP success metrics. What does success look like at the end of the MVP phase? Specify three measurable outcomes that would justify proceeding to full build.

Step 5: Identify the build approach. Should this be a concierge MVP, a fake-door test, a prototype, or a coded product? Recommend the approach that tests the most assumptions with the least build time.
</instructions>

<output_format>
Section 1: Assumption Risk Matrix: table with Assumption, Probability of Being Wrong (1-5), Impact if Wrong (1-5), Risk Score, and Rank columns.
Section 2: Priority Validation Experiment: structured block with Hypothesis, Method, Success Criterion, Time Required, and Estimated Cost.
Section 3: MVP Scope: two lists. IN SCOPE: bullet list of included features. OUT OF SCOPE: bullet list of excluded features with one-line rationale for each exclusion.
Section 4: MVP Success Metrics: three numbered metrics, each with a specific, measurable target.
Section 5: Build Approach Recommendation: one paragraph with recommended approach and rationale.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Validation experiments must be completable within available resources.
- MVP scope must be genuinely minimal. Err on the side of cutting, not including.
- Success metrics must be specific numbers or observable outcomes, not vague indicators.
- Do not recommend building anything that can be tested without building.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Risk scores are mathematically correct (Probability x Impact).
2. Assumptions are ranked correctly by risk score.
3. Validation experiment has all five components (Hypothesis, Method, Success Criterion, Time, Cost).
4. MVP scope has both IN and OUT lists with rationale for exclusions.
5. All three success metrics are specific and measurable.
</evaluation_criteria>
```

---

## Why This Works

The assumption risk matrix forces founders to confront which beliefs are most likely to be wrong and most consequential if wrong, preventing the natural tendency to build features that confirm existing convictions. Separating the validation experiment design from the MVP scope ensures founders test before they build, not as they build.

---

## Sample Output

Assumption Risk Matrix row: Customers will pay £18,000/year | 3 | 5 | 15 | Rank 1, highest priority to validate before any build begins

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
