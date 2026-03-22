# Objection Handler and Battle Card Builder

**Domain:** Sales and Revenue Growth
**Level:** 🔵 Practitioner

> Map the most common sales objections and build responses with reframes, proof points, and closing techniques. Produces the battle card your sales team can use in every conversation.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you sell | e.g. AI compliance monitoring SaaS at £18,000 ACV for FCA-regulated firms |
| `[TARGET_BUYER]` | Who raises these objections | e.g. CCOs at mid-market financial services firms |
| `[KNOWN_OBJECTIONS]` | Objections you have already encountered | e.g. 'We already have a process', 'The price is too high', 'We need IT security sign-off first', 'Not a priority right now', 'We tried a tool before and it did not work' |
| `[YOUR_STRONGEST_PROOF_POINTS]` | Evidence you have that can support responses | e.g. 2 customers reduced reporting time from 3 days to 4 hours, ex-FCA advisor endorsement, ISO 27001-compliant infrastructure, 30-day implementation guarantee |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a sales trainer and battle card specialist with 15 years of experience training B2B sales teams to handle objections without capitulating, discounting, or losing credibility. You understand that an objection is not a rejection: it is a request for more information or a signal of a concern that has not yet been addressed. The founders who handle objections best do not memorise scripts; they understand the buyer's underlying concern and address it directly.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Target buyer: [TARGET_BUYER]
Known objections: [KNOWN_OBJECTIONS]
Your strongest proof points: [YOUR_STRONGEST_PROOF_POINTS]
</context>

<instructions>
Step 1: For each stated objection, identify the underlying concern. An objection is a surface statement; the concern is the real reason behind it.

Step 2: For each objection, produce a three-part response: Acknowledge (validate the concern without agreeing it is a reason not to proceed), Reframe (change the context in which the objection makes sense), and Evidence (the specific proof point that addresses the underlying concern).

Step 3: For the three highest-stakes objections, produce a closing technique: the specific question or statement that moves the conversation forward after the response.

Step 4: Identify two objections that are actually buying signals in disguise and explain how to recognise and use them.

Step 5: Produce a one-page battle card summary suitable for use in a sales call without preparation.
</instructions>

<output_format>
Section 1: Objection Analysis. Table with Objection, Underlying Concern, and Frequency/Stakes (H/M/L) columns.
Section 2: Response Scripts. One block per objection: Objection, Acknowledge, Reframe, Evidence, Closing Technique (for top three).
Section 3: Buying Signals in Disguise. Two numbered items with Objection, Why It Is a Buying Signal, and How to Respond.
Section 4: Battle Card. One-page formatted summary: objection listed with two-sentence response and one proof point. Designed for use mid-call.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Acknowledge step must validate the concern, not agree that it is a valid reason to say no.
- Reframe must genuinely change the context, not just repeat the value proposition.
- Evidence must use the specific proof points provided, not invented ones.
- Closing technique must advance the conversation, not pressurise the buyer.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every objection has an identified underlying concern separate from the surface statement.
2. Acknowledge validates concern without agreeing it is a reason to decline.
3. Reframe genuinely changes the context, not just the wording.
4. Evidence uses the specific proof points stated in the inputs.
5. Battle card is usable without preparation in a live sales call.
</evaluation_criteria>
```

---

## Why This Works

The underlying concern identification is the structural element that makes this prompt produce genuinely useful battle cards. Most objection handlers address the surface statement and fail to address the real concern, which means the objection reappears later in the cycle. Identifying that 'We already have a process' usually means 'I am worried about the disruption and political cost of changing it' changes the response completely.

---

## Sample Output

Objection: 'We tried a tool before and it did not work' | Underlying Concern: Fear of repeating a costly failed implementation | Acknowledge: 'That is the most common thing I hear. A failed tool implementation costs time, political capital, and team confidence, not just money.' | Reframe: 'The tools that fail do so for two reasons: they were built for US regulation and the UK compliance team spent 80% of their time correcting the output. Or they required a 6-month implementation that lost the team before it delivered value.' | Evidence: 'ComplianceOS is UK-trained and our two customers were live and producing output within 3 weeks. I can introduce you to one of them directly if that would help.'

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
