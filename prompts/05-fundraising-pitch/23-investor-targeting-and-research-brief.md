# Investor Targeting and Research Brief

**Domain:** Fundraising, Pitch and Investor Strategy
**Level:** 🔵 Practitioner

> Profile target investors and produce a prioritised outreach list with personalisation angles. Replaces the scattergun approach with a targeted list where every outreach has a specific reason for contact.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_DESCRIPTION]` | What you do and who you serve | e.g. AI compliance monitoring SaaS for UK financial services, targeting CCOs at mid-market FCA-regulated firms |
| `[FUNDING_STAGE_AND_ASK]` | Stage and amount | e.g. Seed round, £1.5m, 18-month runway to Series A readiness |
| `[GEOGRAPHY]` | Where you are based and where you want investors from | e.g. UK-based, prefer UK or European investors with UK portfolio companies |
| `[KNOWN_INVESTOR_NAMES]` | Any investors you have already identified or been introduced to | e.g. Passion Capital, Seedcamp, Notion Capital, one warm intro to Episode 1 |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a fundraising strategist and investor relations advisor with 15 years of experience helping seed and Series A companies build targeted investor pipelines. You understand that the quality of investor targeting determines the quality of the fundraising outcome, and that a warm, researched outreach converts at 10 times the rate of a cold, generic one.
</role>

<context>
Company description: [COMPANY_DESCRIPTION]
Funding stage and ask: [FUNDING_STAGE_AND_ASK]
Geography: [GEOGRAPHY]
Known investor names: [KNOWN_INVESTOR_NAMES]
</context>

<instructions>
Step 1: Define the ideal investor profile for this specific company and stage. What portfolio fit, thesis alignment, cheque size, and geographic focus characterise the perfect investor for this round?

Step 2: Identify investor categories to target. For each category, describe the typical investor in this category, why they are relevant, and the outreach approach most likely to work.

Step 3: For each of the named investors, produce a research brief: thesis, typical cheque size, relevant portfolio companies, the partner most likely to champion this deal, and a specific personalisation angle for the first outreach.

Step 4: Prioritise the investor list into three tiers: Tier 1 (highest fit, pursue first), Tier 2 (strong fit, approach in parallel), Tier 3 (worth a shot, do not lead with).

Step 5: Draft a 100-word cold email template for Tier 1 outreach. Specific, personalised to the investor type, no generic pitch language.
</instructions>

<output_format>
Section 1: Ideal Investor Profile. Five criteria with one-line description each.
Section 2: Investor Categories Table. Columns: Category, Why Relevant, Outreach Approach, Expected Conversion Rate.
Section 3: Named Investor Research Briefs. One structured block per named investor: Thesis, Cheque Size, Relevant Portfolio, Best Contact, Personalisation Angle.
Section 4: Prioritised List. Three tiers, each with investor names and the primary reason for their tier placement.
Section 5: Cold Email Template. 100 words maximum, with [PLACEHOLDER] fields for personalisation.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Named investor details must be accurate to the best of your knowledge. Flag anything uncertain rather than inventing it.
- Personalisation angles must be specific to the investor's stated thesis or portfolio, not generic flattery.
- Cold email must be under 100 words and must not contain generic phrases like "I wanted to reach out" or "I think you would be a great fit."
- Tier placement must be justified, not arbitrary.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Ideal investor profile has five specific criteria.
2. Each named investor has a specific personalisation angle tied to their portfolio or thesis.
3. Three-tier prioritisation is justified for each investor.
4. Cold email is under 100 words and contains no generic opener phrases.
5. Uncertain investor details are flagged, not invented.
</evaluation_criteria>
```

---

## Why This Works

The personalisation angle requirement is the most valuable output. It forces research before outreach and prevents the mass-blast approach that marks a founder as unprepared. The tier system ensures founders spend the most time on the highest-probability investors rather than treating all names equally. The cold email template converts the research into an immediate action.

---

## Sample Output

Named Investor Brief: Seedcamp | Thesis: pre-seed and seed B2B software with European founders, strong on SaaS infrastructure and developer tools; increasing RegTech exposure post-2022 | Cheque: £100-500k at seed | Portfolio: Revolut (early), Phoebe (HR compliance), Factorial | Best Contact: Carlos Espinal (Managing Partner) or Sia Houchangnia (Partner, B2B SaaS focus) | Personalisation: Reference Seedcamp's Phoebe investment and ask whether they see FCA-specific compliance as an adjacent white space to HR compliance automation

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
