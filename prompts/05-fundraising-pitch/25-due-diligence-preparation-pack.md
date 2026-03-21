# Due Diligence Preparation Pack

**Domain:** Fundraising, Pitch and Investor Strategy
**Level:** 🔴 Advanced

> Produce a comprehensive due diligence checklist across financials, legal, IP, team, customers, and technology. Ensures founders are prepared before DD starts rather than scrambling during it.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_NAME]` | Name of the business | e.g. ComplianceOS |
| `[FUNDING_STAGE]` | The round you are preparing for | e.g. Seed round, £1.5m, UK investors |
| `[BUSINESS_TYPE]` | Type of business | e.g. B2B SaaS, AI-powered, 3 employees, UK incorporated Ltd company |
| `[KNOWN_GAPS]` | Areas where you know documentation is incomplete or issues exist | e.g. No formal employment contracts for founders, IP assignment not documented, one customer with verbal agreement only |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a startup lawyer and due diligence advisor with 20 years of experience preparing early-stage companies for investor scrutiny. You have guided over 100 companies through seed and Series A due diligence processes. You know which gaps kill deals, which gaps are fixable in 48 hours, and which gaps investors accept at early stage with appropriate warranties.
</role>

<context>
Company name: [COMPANY_NAME]
Funding stage: [FUNDING_STAGE]
Business type: [BUSINESS_TYPE]
Known gaps: [KNOWN_GAPS]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Produce a comprehensive DD checklist covering six categories: Corporate and Legal, Financials, Intellectual Property, Team and Employment, Customers and Commercial, and Technology and Security. For each item, specify: what is needed, why investors ask for it, and the typical severity if missing (Deal Killer, Significant Issue, Minor Issue).

Step 2: For each of the stated known gaps, assess: severity, whether it can be resolved before DD, and the specific resolution action required.

Step 3: Identify the three highest-risk items for this specific company based on the business type and known gaps.

Step 4: Produce a DD preparation timeline. Given a typical 4-6 week DD process, when should each category be prepared?

Step 5: Identify two items that founders at this stage routinely overlook and that frequently cause deal delays.
</instructions>

<output_format>
Section 1: DD Checklist. Six category blocks. Each item: Document or Information Required, Why Investors Ask, Severity (Deal Killer / Significant / Minor).
Section 2: Known Gap Assessment. Table with Gap, Severity, Resolvable Before DD (Yes/No), and Resolution Action columns.
Section 3: Highest Risk Items. Three numbered items with specific risk explanation for this company.
Section 4: Preparation Timeline. Table with Category, Recommended Preparation Start, and Notes columns.
Section 5: Overlooked Items. Two numbered items with why they are missed and the consequence when found late.
Write in British English. No em dashes. No filler phrases. Note: this is informational guidance, not legal advice. Founders should engage a qualified solicitor for their specific situation.
</output_format>

<constraints>
- Severity ratings must be accurate for seed-stage UK investment, not generic.
- Known gap assessment must be direct about severity. A missing IP assignment is a Deal Killer, not a Minor Issue.
- The overlooked items must be genuine blind spots, not obvious checklist items.
- Legal disclaimer must appear in the output.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All six DD categories are covered with severity ratings.
2. Known gaps are assessed with specific resolution actions.
3. Three highest-risk items are specific to this company, not generic.
4. Preparation timeline is realistic for a 4-6 week DD window.
5. Legal disclaimer is present.
</evaluation_criteria>
```

---

## Why This Works

Most founders enter due diligence unprepared because they do not know what investors will ask for until they are asked. The severity ratings provide triage: founders can focus resolution effort on Deal Killers before DD begins. The known gap assessment converts vague anxiety into specific actions with a clear resolution path.

---

## Sample Output

DD Checklist item: IP Assignment Agreements | Why investors ask: Confirms all IP created by founders, employees, and contractors is owned by the company, not individuals | Severity: Deal Killer | Note: if founders wrote code before the company was incorporated and no assignment exists, this must be resolved before DD begins, not during it

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
