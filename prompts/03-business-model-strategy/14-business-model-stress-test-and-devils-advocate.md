# Business Model Stress-Test and Devil's Advocate

**Domain:** Business Model and Strategy
**Level:** 🔴 Advanced

> Adversarial analysis of a business model. Identify the hidden failure points, market shifts, regulatory changes, and competitive threats that could make the model obsolete. The analysis a sceptical Series A investor runs before they pass.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_MODEL_SUMMARY]` | Full description of the business model including product, customer, revenue, and key assumptions | e.g. B2B SaaS selling FCA compliance monitoring to mid-market financial services firms at £18k ACV; assuming 3-day sales cycle, CCO budget authority, 80% gross margin, 10% monthly churn |
| `[MOST_CONFIDENT_ASSUMPTIONS]` | The assumptions you are most confident about | e.g. FCA compliance complexity is increasing, CCOs have growing budgets, manual processes are genuinely painful |
| `[KNOWN_RISKS]` | Risks you are already aware of | e.g. FCA digitalises compliance reporting natively, making third-party tools redundant; US RegTech giants enter UK market |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a seasoned venture capitalist and former operating executive who has seen 200+ business models succeed and fail. Your role here is to act as the most rigorous sceptic in the room, not to be negative for its own sake, but to surface every assumption, structural flaw, and market risk that the founder has not yet confronted. You are being paid to be right, not to be encouraging.
</role>

<context>
Business model summary: [BUSINESS_MODEL_SUMMARY]
Most confident assumptions: [MOST_CONFIDENT_ASSUMPTIONS]
Known risks: [KNOWN_RISKS]
</context>

<instructions>
Think through this step by step. Approach this as an adversarial exercise.

Step 1: Identify five hidden assumptions embedded in this business model that the founder has not explicitly stated. For each, assess the probability of the assumption being wrong (Low/Medium/High) and the impact if wrong (Low/Medium/High).

Step 2: Identify the three most dangerous structural failure points in this model. A structural failure point is a characteristic of the model itself (not an external event) that could cause it to fail at scale.

Step 3: Identify two plausible market shifts (regulatory changes, technology shifts, or demand changes) that would materially damage this model within 36 months.

Step 4: Construct the strongest possible bear case for this business. Write it as a VC partner would present it to their partnership: specific, evidenced, and designed to convince sceptics that this investment should be passed.

Step 5: Identify the single change to the business model that would most effectively address the bear case, and the trade-off it creates.
</instructions>

<output_format>
Section 1: Hidden Assumption Audit: table with Assumption, Probability Wrong (L/M/H), Impact if Wrong (L/M/H), and Consequence columns.
Section 2: Structural Failure Points: three numbered paragraphs, each identifying a failure point with specific explanation.
Section 3: Market Shift Scenarios: two structured blocks with Shift Description, Trigger, Timeline (months), and Impact on Model columns.
Section 4: Bear Case: one paragraph written from the perspective of a sceptical VC partner presenting a pass recommendation.
Section 5: Model-Strengthening Move: one paragraph naming the change and the trade-off it creates.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- The bear case must be specific and evidence-based. Generic risk statements do not qualify.
- Hidden assumptions must be genuinely non-obvious. Do not restate the known risks provided.
- Structural failure points must be about the model's internal logic, not external events.
- The model-strengthening move must create a genuine trade-off, not be a free improvement.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Five hidden assumptions are identified and none overlap with the stated known risks.
2. Three structural failure points are about model logic, not external events.
3. Bear case is written from a specific VC perspective, not as a bullet list of risks.
4. Model-strengthening move names a specific trade-off.
5. No generic risk statements that apply to any business.
</evaluation_criteria>
```

---

## Why This Works

Most founders never subject their model to genuine adversarial analysis before investor due diligence. Constructing the bear case before the first VC meeting allows founders to either pre-empt the objections or change the model before it is too late. The structural failure point analysis is the component most founders find the most uncomfortable and most valuable.

---

## Sample Output

Hidden Assumption row: CCOs have unilateral budget authority for compliance tooling up to £25,000 | Probability Wrong: High | Impact if Wrong: High | Consequence: Sales cycle extends from 3 days to 90+ days when IT security, procurement, and finance approval are required, fundamentally changes CAC and payback period

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
