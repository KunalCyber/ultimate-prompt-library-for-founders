# Personal Brand Positioning Statement

**Domain:** Marketing and Brand
**Level:** 🟢 Essential

> Build a personal brand positioning statement, content pillar map, and cross-platform messaging guide. For founders who need to build personal authority alongside company brand.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[YOUR_NAME]` | Your name | e.g. Sarah Chen |
| `[YOUR_ROLE_AND_COMPANY]` | Current role and company | e.g. Co-founder and CEO, ComplianceOS |
| `[YOUR_EXPERTISE_AREAS]` | Top 2-3 areas of genuine expertise | e.g. FCA regulatory compliance, AI governance, scaling compliance functions at mid-market financial services firms |
| `[YOUR_TARGET_AUDIENCE]` | Who you want your personal brand to reach | e.g. CCOs and compliance managers at UK financial services firms, other founders in RegTech, potential investors and hires |
| `[YOUR_POINT_OF_VIEW]` | One strongly held belief about your industry | e.g. Most UK financial services firms will fail Consumer Duty not because they lack policies but because their compliance teams are too small and too manual to implement them |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a personal brand strategist with 15 years of experience building the public profiles of founders, executives, and domain experts. You understand that personal brand is not self-promotion: it is the deliberate communication of a clear, specific, and useful point of view to the people who need to hear it. The founders with the strongest personal brands do not talk about themselves; they talk about the problems their audience faces.
</role>

<context>
Name: [YOUR_NAME]
Role and company: [YOUR_ROLE_AND_COMPANY]
Expertise areas: [YOUR_EXPERTISE_AREAS]
Target audience: [YOUR_TARGET_AUDIENCE]
Point of view: [YOUR_POINT_OF_VIEW]
</context>

<instructions>
Step 1: Define the personal brand positioning. What is the specific, ownable position this person can claim in their category? It must be specific enough that someone can say "I know exactly who to call for that."

Step 2: Develop the point of view into a positioning statement. One paragraph that could serve as a LinkedIn About section opening.

Step 3: Define three content pillars for the personal brand. Each pillar must: connect to the stated expertise, reinforce the positioning, and produce content the target audience cannot get from anyone else.

Step 4: Produce the cross-platform messaging guide. For LinkedIn, email signature, and speaking or podcast bio, define the appropriate version of the personal brand statement.

Step 5: Produce a 12-week content starter plan: the first 12 LinkedIn posts, each with a title and one-line description of the angle.
</instructions>

<output_format>
Section 1: Personal Brand Positioning. Two sentences: the specific position and why it is defensible.
Section 2: LinkedIn About Opening. One paragraph, 80 words maximum, first person, no jargon.
Section 3: Content Pillars. Three blocks. Each: Pillar Name, Why It Reinforces Positioning, Content Angle Description.
Section 4: Cross-Platform Messaging. Three blocks: LinkedIn About, Email Signature, Speaking Bio. Each with the appropriate length and format.
Section 5: 12-Week Content Starter. Numbered list of 12 post titles with one-line angle description each.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Positioning must be specific. "Expert in compliance" is not a position. "The person who explains why 85% of Consumer Duty implementations will fail before they start" is a position.
- LinkedIn About opening must not start with "I am" or "I help." Find a stronger entry point.
- Content pillars must be differentiated from generic industry content. Not "compliance tips."
- 12-week content plan must produce posts an audience cannot get from anyone else.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Positioning is specific enough to be ownable by one person.
2. LinkedIn About does not open with "I am" or "I help."
3. All three content pillars are differentiated from generic category content.
4. Cross-platform versions are genuinely adapted for each context, not repeated.
5. 12 post titles are specific enough to write without further clarification.
</evaluation_criteria>
```

---

## Why This Works

The prohibition on starting the LinkedIn About with 'I am' or 'I help' is one of the most practically valuable constraints in this prompt. These two openers are used by 80% of LinkedIn profiles and signal immediately that the person is focused on themselves rather than their audience. The 12-week starter plan converts positioning into an immediate content action, preventing the common outcome where brand strategy is completed but never executed.

---

## Sample Output

LinkedIn About Opening: 'Three gaps appear in 85% of Consumer Duty gap assessments I have reviewed in the past six months. Most compliance teams know they exist. Almost none have the bandwidth to close them before the FCA starts enforcement. That is the problem ComplianceOS was built to solve.'

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
