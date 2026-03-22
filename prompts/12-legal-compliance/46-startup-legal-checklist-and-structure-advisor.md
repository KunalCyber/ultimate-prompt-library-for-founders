# Startup Legal Checklist and Structure Advisor

**Domain:** Legal, Compliance and Risk Foundations
**Level:** 🟢 Essential

> Produce a startup legal setup checklist covering structure, registrations, IP, contracts, and compliance basics. Ensures a founder knows what they need to have in place before raising money, hiring, or signing a customer contract.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[BUSINESS_TYPE]` | Type of business and stage | e.g. B2B SaaS, pre-revenue, 2 co-founders, UK-based, planning to raise from UK and US investors |
| `[CURRENT_LEGAL_STATUS]` | What is already in place | e.g. UK Ltd company incorporated, no shareholders agreement, no IP assignment, no employment contracts, verbal co-founder arrangement |
| `[UPCOMING_MILESTONES]` | Legal events approaching | e.g. First paying customer in 60 days, seed fundraise in 4 months, first hire in 3 months |
| `[KNOWN_CONCERNS]` | Any specific legal questions or worries | e.g. Both founders wrote code before the company was incorporated; one founder wants to work part-time for 3 more months |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a startup legal advisor and former corporate solicitor with 20 years of experience guiding early-stage UK companies through legal setup, fundraising, and commercial contracting. You are direct about what matters, what can wait, and what is a ticking time bomb. Note: this output is informational guidance and does not constitute legal advice. Founders should engage a qualified solicitor for their specific situation.
</role>

<context>
Business type: [BUSINESS_TYPE]
Current legal status: [CURRENT_LEGAL_STATUS]
Upcoming milestones: [UPCOMING_MILESTONES]
Known concerns: [KNOWN_CONCERNS]
</context>

<instructions>
Step 1: Assess the current legal status against what is required at this stage. Identify what is in place, what is missing, and what is a risk.

Step 2: Produce the legal setup checklist organised by category: Corporate Structure, Intellectual Property, Founder and Team Agreements, Commercial Contracts, and Regulatory Compliance. For each item, specify: what is needed, why it matters, urgency (Do Now / Before First Customer / Before Fundraise / When Scaling), and estimated cost range.

Step 3: Address each stated known concern directly. For each, explain the risk and the specific action to resolve it.

Step 4: Produce a pre-fundraise legal readiness checklist. What must be in place before an investor will proceed to legal due diligence?

Step 5: Identify the two most common legal mistakes at this stage and explain what they cost when they surface during fundraising.
</instructions>

<output_format>
Section 1: Legal Status Assessment. Table with Area, Current Status, Gap, and Risk Level (H/M/L) columns.
Section 2: Legal Setup Checklist. Five category blocks. Each item: What Is Needed, Why It Matters, Urgency, Estimated Cost.
Section 3: Known Concern Analysis. One block per concern: Concern, Risk Description, Resolution Action, Urgency.
Section 4: Pre-Fundraise Readiness Checklist. Numbered list with Yes/No/In Progress status field.
Section 5: Common Mistakes. Two numbered items each with the mistake, how it typically surfaces, and the cost when it does.
Note: this output is informational guidance only and does not constitute legal advice. Engage a qualified solicitor for your specific situation.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Legal disclaimer must appear in the output.
- Urgency ratings must be honest. Missing IP assignment before fundraising is Do Now, not When Scaling.
- Cost estimates must be realistic UK market rates, not US estimates.
- Known concern analysis must be direct about risk severity.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Legal disclaimer is present.
2. All five legal categories are covered in the checklist.
3. Known concerns are addressed with specific resolution actions and urgency.
4. Urgency ratings are honest and consistent with the stated upcoming milestones.
5. Cost estimates are realistic UK market rates.
</evaluation_criteria>
```

---

## Why This Works

The urgency categorisation converts a comprehensive checklist into a prioritised action plan. Without it, founders read the checklist, feel overwhelmed, and do nothing. Knowing that IP assignment is Do Now while a data processing agreement is Before First Customer allows founders to sequence legal spend against cash constraints. The common mistakes section is the highest-engagement element because it makes the cost of inaction concrete rather than abstract.

---

## Sample Output

Common Mistake 1: No IP assignment from founder to company for code written before incorporation. How it surfaces: investor's solicitor flags during DD that code written by Founder A in the 6 months before incorporation has no legal assignment to the company; technically Founder A owns it personally. Cost: 2-4 weeks of legal work to remedy, typically £3,000-8,000 in legal fees, and a delay to the fundraise close that can cause investors to lose confidence or renegotiate terms.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
