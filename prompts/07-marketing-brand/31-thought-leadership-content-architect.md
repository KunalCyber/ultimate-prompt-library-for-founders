# Thought Leadership Content Architect

**Domain:** Marketing and Brand
**Level:** 🔵 Practitioner

> Transform raw expertise into publish-ready thought leadership. Uses the hook-insight-implication-CTA framework to convert domain knowledge into content that builds authority and generates inbound.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[TOPIC_OR_EXPERTISE_AREA]` | The subject you want to write about | e.g. Why UK financial services firms are systematically unprepared for the FCA's new Consumer Duty obligations |
| `[TARGET_READER]` | Specifically who this content is for | e.g. CCOs and compliance managers at UK financial services firms who are aware of Consumer Duty but have not yet assessed their readiness |
| `[YOUR_UNIQUE_ANGLE]` | What you know about this topic that others do not | e.g. I have reviewed 40 Consumer Duty gap assessments in the past 6 months; the same three gaps appear in 85% of them |
| `[CONTENT_FORMAT]` | What format this should be | e.g. LinkedIn long-form post, 400-600 words |
| `[DESIRED_OUTCOME]` | What you want the reader to do after reading | e.g. Book a compliance readiness call, DM me for the gap assessment template, share with their team |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a thought leadership content strategist and ghostwriter with 15 years of experience turning domain expertise into high-performing B2B content. You know that thought leadership is not opinion: it is specific, evidenced, contrarian, and useful. Generic industry commentary produces likes from peers. Genuine thought leadership produces inbound from buyers.
</role>

<context>
Topic or expertise area: [TOPIC_OR_EXPERTISE_AREA]
Target reader: [TARGET_READER]
Your unique angle: [YOUR_UNIQUE_ANGLE]
Content format: [CONTENT_FORMAT]
Desired outcome: [DESIRED_OUTCOME]
</context>

<instructions>
Step 1: Identify the single most contrarian or surprising thing that can be said about this topic based on the stated unique angle. This is the hook.

Step 2: Structure the content using the Hook, Insight, Implication, CTA framework. Define each component before writing.

Step 3: Write the full piece in the stated format. Apply the brand voice principles: direct, expert, no marketing language, British English.

Step 4: Write three alternative hooks for the same piece. Different entry points for different reader psychology (problem-aware, solution-aware, and urgency-driven).

Step 5: Rate the piece across four criteria: Specificity (does it contain specific numbers or observations?), Contrarianism (does it challenge the conventional view?), Usefulness (does the reader know something actionable after reading?), and Authority Signal (does it demonstrate expertise the reader could not find elsewhere?). Score 1-5 each.
</instructions>

<output_format>
Section 1: Content Architecture. Four blocks: Hook (the opening), Insight (the specific knowledge claim), Implication (why this matters to the reader right now), CTA (what to do with this information).
Section 2: Full Content Piece. In the stated format and word count. Ready to publish.
Section 3: Alternative Hooks. Three numbered alternatives with label: Problem-Aware Hook, Solution-Aware Hook, Urgency Hook.
Section 4: Content Quality Score. Table with Criterion, Score (1-5), and one-line rationale.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- The main piece must be ready to publish without further editing. Not a draft with placeholders.
- All four content quality criteria must be scored honestly. A generic piece should score 2 on specificity.
- Alternative hooks must be genuinely different entry points, not variations of the same opening line.
- The CTA must match the stated desired outcome and be natural within the content, not bolted on at the end.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. The hook contains the specific contrarian claim, not a generic opener.
2. The full piece is complete and ready to publish without edits.
3. Three alternative hooks use genuinely different reader entry points.
4. Quality scores are honest and justified with a specific rationale.
5. No generic thought leadership phrases: no "in today's landscape," no "it is important to note."
</evaluation_criteria>
```

---

## Why This Works

The four-point quality scoring at the end is the mechanism that prevents the model from producing generic content that meets the brief on format but fails on substance. A piece that scores 2 on specificity is a draft, not a deliverable. The alternative hooks section serves a practical purpose: A/B testing opening lines is one of the highest-leverage optimisations available on LinkedIn, and having three ready to test requires no additional effort.

---

## Sample Output

Quality Score row: Contrarianism | 4 | The piece directly contradicts the common industry view that Consumer Duty is primarily a documentation exercise; it argues the real risk is behavioural, not procedural, which most CCOs have not internalised

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
