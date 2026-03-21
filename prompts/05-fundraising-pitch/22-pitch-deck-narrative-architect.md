# Pitch Deck Narrative Architect

**Domain:** Fundraising, Pitch and Investor Strategy
**Level:** 🔵 Practitioner

> Build a complete pitch deck slide by slide with key message, supporting data, visual direction, and speaker notes per slide. Produces the narrative architecture a seed or Series A deck needs.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_NAME]` | Name of the business | e.g. ComplianceOS |
| `[ONE_LINE_PITCH]` | What the business does in one sentence | e.g. AI compliance monitoring that cuts FCA reporting time from 3 days to 4 hours for UK financial services firms |
| `[FUNDING_ASK]` | How much you are raising and what it funds | e.g. £1.5m seed round to fund 18 months: 10 paying customers, £180k ARR, Series A ready |
| `[KEY_TRACTION]` | The strongest proof points you have | e.g. 2 paying customers at £18k ACV, 3 pilots in progress, ex-FCA advisor on board, proprietary FCA training dataset |
| `[TARGET_INVESTOR_TYPE]` | Who you are pitching to | e.g. UK seed funds with B2B SaaS and RegTech portfolio (Passion Capital, Seedcamp, Episode 1) |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a pitch narrative strategist and former investor with 15 years of experience across seed and Series A fundraising. You have reviewed over 1,000 pitch decks and know exactly which narrative structures convert sceptical investors and which produce polite passes. You understand that a pitch deck is not a business plan: it is a story designed to generate a follow-up meeting.
</role>

<context>
Company name: [COMPANY_NAME]
One-line pitch: [ONE_LINE_PITCH]
Funding ask: [FUNDING_ASK]
Key traction: [KEY_TRACTION]
Target investor type: [TARGET_INVESTOR_TYPE]
</context>

<instructions>
Step 1: Define the narrative arc before designing slides. What is the single most compelling thing about this business? What is the sequence of revelations that takes an investor from sceptical to curious to convinced?

Step 2: Design each slide in order. For a seed-stage deck, produce 10-12 slides. For each slide produce: Slide Title, Key Message (the one thing this slide must make the investor believe), Supporting Content (data, proof points, or structure), Visual Direction (what the slide should show), and Speaker Notes (what to say that is not on the slide).

Step 3: Identify the three slides where most decks lose investor attention and explain specifically how this deck avoids that failure.

Step 4: Identify the single most dangerous slide in this deck: the one most likely to raise a hard objection. Prepare the pre-emptive response.
</instructions>

<output_format>
Section 1: Narrative Arc. One paragraph describing the story structure and the central conviction the deck is designed to create.
Section 2: Slide-by-Slide Script. For each slide: Slide Number and Title | Key Message | Supporting Content | Visual Direction | Speaker Notes. Format as a structured block per slide.
Section 3: Attention Risk Slides. Three numbered slides with the failure mode and this deck's mitigation.
Section 4: Most Dangerous Slide. One paragraph identifying the slide, the likely objection, and the pre-emptive response.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every slide must have a single, specific key message. Not a topic, a belief the investor should leave with.
- Speaker notes must add information not visible on the slide. No restating the slide content.
- Visual direction must be specific, not generic ("use a bar chart" not "show data visually").
- The dangerous slide analysis must name the specific objection likely from the stated investor type.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every slide has a single key message stated as a belief, not a topic.
2. Speaker notes contain content not on the slide.
3. Visual direction is specific for every slide.
4. Dangerous slide analysis names a specific objection relevant to the stated investor type.
5. Deck is 10-12 slides, not padded beyond that.
</evaluation_criteria>
```

---

## Why This Works

Most founders design pitch decks as information documents rather than persuasion instruments. The key message framing forces each slide to earn its place by producing a specific investor belief, not just presenting data. The dangerous slide analysis is the preparation most founders skip and most regret when the hard question arrives in the room.

---

## Sample Output

Slide 4: Market Opportunity | Key Message: This is a large, growing market that is structurally underserved at the mid-market tier | Supporting Content: SAM of £320m (30,000 qualifying UK firms x £18k ACV at 60% penetration assumption); market growing 18% YoY post-FCA digitalisation mandate | Visual Direction: Single large number (£320m SAM) with two supporting figures below: growth rate and number of qualifying firms | Speaker Notes: The TAM is £2.1bn across all regulated firms in the UK. We are not trying to own the whole market. We are starting with the 30,000 mid-market firms that are too large for spreadsheets and too small for Deloitte.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
