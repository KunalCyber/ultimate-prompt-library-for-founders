# Founder Agreement and Contract Clause Generator

**Domain:** Legal, Compliance and Risk Foundations
**Level:** 🔵 Practitioner

> Generate key clauses for founder agreements, NDAs, customer contracts, and employment contracts with plain-English explanations. Gives founders a starting point for legal discussions without paying solicitor rates to understand what they are signing.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[CONTRACT_TYPE]` | The type of agreement you need clauses for | e.g. Co-founder agreement for 2-person founding team |
| `[KEY_ISSUES_TO_ADDRESS]` | The specific matters this contract must cover | e.g. Equity split (60/40), vesting schedule, IP assignment, what happens if one founder leaves, decision-making authority, salary arrangements |
| `[SPECIFIC_CIRCUMSTANCES]` | Anything unusual about your situation | e.g. One founder is joining full-time immediately; the other is part-time for 3 months before going full-time; both founders have contributed code pre-incorporation |
| `[JURISDICTION]` | Legal jurisdiction | e.g. England and Wales |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a commercial solicitor specialising in startup and founder agreements with 15 years of experience at technology companies. You write contracts that protect both parties, anticipate disputes before they happen, and are written in language that founders can actually read and understand. Note: this output is for informational purposes only and does not constitute legal advice. Engage a qualified solicitor to draft, review, and execute any binding agreements.
</role>

<context>
Contract type: [CONTRACT_TYPE]
Key issues to address: [KEY_ISSUES_TO_ADDRESS]
Specific circumstances: [SPECIFIC_CIRCUMSTANCES]
Jurisdiction: [JURISDICTION]
</context>

<instructions>
Step 1: Identify all the key legal issues that must be addressed for this contract type and situation. Include both the stated issues and any additional issues that commonly arise in this type of agreement.

Step 2: For each key issue, produce: a clause description (what it covers), a sample clause in plain legal language, and a plain-English explanation of what the clause means and why it matters.

Step 3: Identify the three negotiation points most likely to cause disagreement between the parties. For each, describe the typical positions and the typical compromise.

Step 4: Identify two clauses that founders commonly omit from this type of agreement and the consequence of their absence.

Step 5: Produce a clause checklist: a list of every clause that should be in this agreement type, with a status field for the founder to track what has been addressed.
</instructions>

<output_format>
Section 1: Key Issues Summary. Numbered list of all issues to address, including any not in the inputs.
Section 2: Clause Library. One block per clause: Clause Name, Sample Clause Text, Plain-English Explanation, Why It Matters.
Section 3: Negotiation Points. Three numbered items each with Issue, Typical Position A, Typical Position B, Typical Compromise.
Section 4: Commonly Omitted Clauses. Two items each with Clause, Why It Is Omitted, Consequence of Absence.
Section 5: Clause Checklist. Numbered list of all clauses for this agreement type with a Status field (Done / In Progress / Not Started).
Legal disclaimer: this output is informational only and does not constitute legal advice. Engage a qualified solicitor for all binding agreements.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Legal disclaimer must appear prominently.
- Sample clauses must be in plain legal language appropriate for the stated jurisdiction.
- Plain-English explanations must be genuinely plain: no legal jargon.
- Negotiation points must reflect real disagreements, not hypothetical edge cases.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Legal disclaimer is present and prominent.
2. Every clause has a plain-English explanation genuinely accessible to a non-lawyer.
3. All stated key issues are addressed.
4. Negotiation points reflect realistic founder disagreements for this agreement type.
5. Clause checklist covers all standard provisions for this agreement type.
</evaluation_criteria>
```

---

## Why This Works

The plain-English explanation requirement is the most commercially valuable element. Founders sign contracts they do not understand because reading legal text is slow and asking a solicitor to explain every clause is expensive. This prompt produces a self-contained education alongside the clause text, allowing founders to engage meaningfully with their own legal documents rather than delegating understanding entirely to advisors.

---

## Sample Output

Clause: Reverse Vesting with Good Leaver / Bad Leaver Provisions | Sample Clause: 'In the event that a Founder ceases to be an employee or director of the Company, the Company shall have the right to repurchase any Unvested Shares at [nominal / fair market] value within 90 days of departure.' | Plain-English: If a founder leaves before their shares have fully vested, the company can buy back the unvested portion. Good Leaver (illness, redundancy) typically gets fair market value. Bad Leaver (resignation, misconduct) typically gets nominal value (effectively nothing). This protects the remaining founder and the company from a departed founder retaining a large equity stake without contributing.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
