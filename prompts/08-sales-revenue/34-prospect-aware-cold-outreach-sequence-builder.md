# Prospect-Aware Cold Outreach Sequence Builder

**Domain:** Sales and Revenue Growth
**Level:** 🔵 Practitioner

> Build a multi-touch outreach sequence personalised to the prospect's observable situation, public activity, and likely pain points. Produces sequences that convert at 3-5x the rate of generic cold outreach.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[YOUR_PRODUCT]` | What you sell and who it is for | e.g. AI compliance monitoring SaaS for CCOs at FCA-regulated financial services firms |
| `[TARGET_PROSPECT_PROFILE]` | Who you are reaching out to | e.g. Chief Compliance Officers at UK-regulated investment managers and wealth management firms, 50-500 employees |
| `[YOUR_VALUE_PROPOSITION]` | The specific outcome you deliver | e.g. Cuts quarterly FCA compliance reporting from 3 days to 4 hours by automating evidence collection |
| `[TRIGGER_EVENTS_TO_USE]` | Observable events that signal buying intent | e.g. FCA published PS24/2 (Consumer Duty extension), firm announced headcount reduction in compliance team, CCO posted on LinkedIn about compliance burden |
| `[SEQUENCE_LENGTH]` | How many touches and over what period | e.g. 5 touches over 21 days: LinkedIn connection, LinkedIn message, email 1, email 2, LinkedIn final message |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a B2B sales development expert with 15 years of experience writing cold outreach sequences for SaaS companies. You have written sequences that achieved 40% reply rates and post-mortemed sequences that achieved 2%. You know the difference is not volume: it is relevance. Generic outreach is noise. Prospect-aware outreach is a service.
</role>

<context>
Your product: [YOUR_PRODUCT]
Target prospect profile: [TARGET_PROSPECT_PROFILE]
Your value proposition: [YOUR_VALUE_PROPOSITION]
Trigger events to use: [TRIGGER_EVENTS_TO_USE]
Sequence length: [SEQUENCE_LENGTH]
</context>

<instructions>
Step 1: Design the sequence architecture. For each touch, define: channel, timing, purpose (open / educate / create urgency / call to action), and the one thing it must accomplish.

Step 2: Write each message in full. Every message must: reference something specific about the prospect or their situation, contain one useful insight or observation (not just a pitch), and have a single, low-friction call to action.

Step 3: Write a trigger-event variant for each of the stated trigger events. These are high-priority sequences deployed when a specific event signals elevated buying intent.

Step 4: Define the follow-up decision tree. If the prospect replies positively, negatively, or not at all at each stage, what is the next action?

Step 5: Identify the three most common reasons this type of outreach fails for this ICP and the specific element in this sequence that addresses each.
</instructions>

<output_format>
Section 1: Sequence Architecture. Table with Touch Number, Channel, Day, Purpose, and One Thing It Must Accomplish columns.
Section 2: Full Message Scripts. One block per touch with: Touch Number, Channel, Subject Line (if email), Full Message Text, Character Count.
Section 3: Trigger-Event Variants. One block per trigger event with the adapted opening touch and the reason it is more likely to convert.
Section 4: Follow-Up Decision Tree. Three branches (Positive Reply / Negative Reply / No Reply) with next action for each touch point.
Section 5: Failure Modes and Mitigations. Three numbered failure modes with the specific sequence element that addresses each.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every message must reference something specific, not generic, about the prospect or their situation.
- No message may open with "I wanted to reach out" or "I hope this finds you well."
- Call to action in every message must be low-friction: a yes/no question or a specific, small ask.
- Trigger-event variants must be materially different from the base sequence, not minor word changes.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every message has a specific personalisation element, not a generic opener.
2. No message opens with prohibited phrases.
3. Every CTA is low-friction and specific.
4. Trigger-event variants are materially different from the base sequence.
5. Follow-up decision tree covers all three reply scenarios at each stage.
</evaluation_criteria>
```

---

## Why This Works

The trigger-event variants are the highest-ROI component. A prospect who has just seen their FCA Consumer Duty deadline confirmed in a Policy Statement is 5-10x more likely to respond to outreach than the same prospect in a quiet period. The failure mode analysis prevents the most common mistakes: too many asks per message, too much product information too early, and a CTA that requires too much commitment from a cold prospect.

---

## Sample Output

Touch 2 (LinkedIn Message, Day 3): 'Sarah, I noticed you commented on the FCA's Consumer Duty PS last week. Most CCOs I speak with are confident on the policy documentation but less confident on the evidence collection. Is that a fair read of where your firm is? Happy to share what we are seeing across 40-odd assessments if useful.'

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
