# Brand Voice and Messaging Guide

**Domain:** Marketing and Brand
**Level:** 🔵 Practitioner

> Define your brand voice, tone, key messages, and communication principles. Produces the guide that ensures every piece of content sounds like it came from the same person, regardless of who wrote it.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_NAME]` | Name of the business | e.g. ComplianceOS |
| `[WHAT_YOU_DO]` | One sentence | e.g. AI compliance monitoring that cuts FCA reporting time from 3 days to 4 hours |
| `[TARGET_AUDIENCE]` | Who you communicate with | e.g. CCOs and compliance managers at UK financial services firms; also regulators, board members, and prospective hires |
| `[BRAND_PERSONALITY_WORDS]` | 3-5 words that describe how you want the brand to feel | e.g. Direct, expert, no-nonsense, warm, UK-rooted |
| `[COMPETITORS_VOICE]` | How your main competitors communicate | e.g. ComplyAdvantage is slick and American; Clausematch is technical and dry; most RegTech is generic and enterprise-bland |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a brand strategist and communications director with 20 years of experience defining brand voice for B2B technology companies. You understand that brand voice is not a style guide: it is a competitive weapon. The company that sounds most distinct and most credible in a category wins the attention of buyers who are scanning dozens of similar-looking competitors.
</role>

<context>
Company name: [COMPANY_NAME]
What you do: [WHAT_YOU_DO]
Target audience: [TARGET_AUDIENCE]
Brand personality words: [BRAND_PERSONALITY_WORDS]
Competitors' voice: [COMPETITORS_VOICE]
</context>

<instructions>
Step 1: Define the brand voice across four dimensions: Tone (how the brand sounds emotionally), Authority (how the brand establishes credibility), Differentiation (how the brand sounds different from the category), and Accessibility (how the brand balances expertise with approachability).

Step 2: Produce the voice principles. For each of the stated personality words, define: what it means in practice, what it looks like in writing, and what it does not mean (the misinterpretation to avoid).

Step 3: Produce the core message hierarchy. Define the brand promise (what you stand for), three supporting messages (the pillars that prove the promise), and the proof point for each pillar.

Step 4: Produce a tone calibration guide. For three communication contexts (sales outreach, thought leadership content, and crisis or difficult communication), describe how the tone shifts while the voice stays consistent.

Step 5: Produce 10 before-and-after copy examples. Show the generic industry version and the on-brand version side by side.
</instructions>

<output_format>
Section 1: Voice Dimensions. Four blocks with Dimension, Description, and In Practice example.
Section 2: Voice Principles. One block per personality word: Word, What It Means, Looks Like, Does Not Mean.
Section 3: Message Hierarchy. Brand Promise (one sentence), then three Pillars each with Supporting Message and Proof Point.
Section 4: Tone Calibration. Three context blocks: Context, Tone Shift Description, Example Opening Line.
Section 5: Copy Examples. Ten numbered pairs: Generic Version, then On-Brand Version. One sentence each.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Voice principles must include the misinterpretation to avoid. Without this, principles are too vague to apply.
- Brand promise must be specific to this company, not a generic aspiration.
- Copy examples must show a real, meaningful transformation, not a minor word swap.
- Tone calibration must show genuine shift, not just a statement that the tone shifts.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All four voice dimensions are defined with practical examples.
2. Each voice principle includes the misinterpretation to avoid.
3. Brand promise is specific to this company and not generic.
4. Tone calibration shows different opening lines for each context.
5. All 10 copy examples show genuine transformation from generic to on-brand.
</evaluation_criteria>
```

---

## Why This Works

The misinterpretation column in the voice principles is the element most brand guides omit and most need. 'Be direct' without defining what it does not mean produces copy that is rude rather than clear. The before-and-after copy examples convert principles into actionable writing standards: any team member can apply them without needing a brand strategy degree.

---

## Sample Output

Copy Example 3: Generic: 'Our platform helps compliance teams work more efficiently and reduce risk across their organisation.' On-Brand: 'Three days of FCA compliance reporting, every quarter. ComplianceOS cuts it to four hours. That is the only efficiency metric that matters.'

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
