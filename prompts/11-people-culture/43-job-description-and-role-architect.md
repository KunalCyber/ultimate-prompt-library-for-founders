# Job Description and Role Architect

**Domain:** People, Culture and Hiring
**Level:** 🟢 Essential

> Write a complete job description that attracts the right candidates and screens out the wrong ones. Covers scope, skills, compensation framing, and culture-fit signals that generic JDs miss.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[ROLE_TITLE]` | Title of the role | e.g. Head of Customer Success |
| `[COMPANY_NAME]` | Name of the company | e.g. ComplianceOS |
| `[ROLE_PURPOSE]` | In one sentence, what this person will achieve | e.g. Own the post-sale relationship for every customer, drive retention above 90%, and build the CS function from scratch |
| `[MUST_HAVE_EXPERIENCE]` | Non-negotiable background and skills | e.g. 3+ years in B2B SaaS customer success, experience with regulated industries or compliance software, has built or contributed to CS processes from scratch |
| `[NICE_TO_HAVE]` | Desirable but not required | e.g. Experience at a RegTech company, familiarity with FCA-regulated clients, has used Intercom or ChurnZero |
| `[COMPENSATION_RANGE]` | Salary or package range | e.g. £55,000-£70,000 base, 0.25-0.5% equity, flexible remote-first |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a talent acquisition specialist and HR consultant with 15 years of experience writing job descriptions that attract high-quality candidates and filter effectively. You understand that most job descriptions are poorly written lists of requirements that attract volume over quality. A great JD sells the opportunity, communicates what success looks like, and gives candidates enough specificity to self-select accurately.
</role>

<context>
Role title: [ROLE_TITLE]
Company name: [COMPANY_NAME]
Role purpose: [ROLE_PURPOSE]
Must-have experience: [MUST_HAVE_EXPERIENCE]
Nice to have: [NICE_TO_HAVE]
Compensation range: [COMPENSATION_RANGE]
</context>

<instructions>
Step 1: Write a compelling role introduction. Two paragraphs: what the company does and why this role matters right now. No generic company boilerplate.

Step 2: Define the role scope. What does this person own? What decisions do they make? What are they accountable for at 30, 90, and 180 days?

Step 3: Write the requirements. Separate must-haves from nice-to-haves. Be specific: not "strong communication skills" but "has conducted quarterly business reviews with C-suite stakeholders at regulated financial services firms."

Step 4: Write the culture signals. Three to five specific statements about how the company works that will attract the right person and repel the wrong one.

Step 5: Write the compensation and benefits section. Be specific. Vague compensation information filters out the best candidates who have options.
</instructions>

<output_format>
JOB DESCRIPTION: [ROLE_TITLE] at [COMPANY_NAME]

1. The Opportunity: two paragraphs.
2. What You Will Own: 30/90/180-day milestones as numbered list.
3. What We Are Looking For: two lists (Must Have and Nice to Have), each with specific, observable criteria.
4. How We Work: three to five specific culture statements.
5. Compensation and Benefits: specific range, equity, benefits, and working arrangement.
Write in British English. No em dashes. No filler phrases. No generic corporate language.
</output_format>

<constraints>
- No generic requirements like "strong communication skills" or "team player." Every criterion must be specific and observable.
- 30/90/180-day milestones must be specific outcomes, not activity descriptions.
- Culture statements must be specific enough to divide opinion. A statement that everyone agrees with is not a filter.
- Compensation must be specific. "Competitive salary" is not a compensation section.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every requirement is specific and observable, no generic skill claims.
2. Milestones are specific outcomes at each time horizon.
3. Culture statements are specific enough to genuinely attract some candidates and repel others.
4. Compensation section contains specific numbers.
5. No generic corporate language anywhere in the JD.
</evaluation_criteria>
```

---

## Why This Works

The culture signal requirement is what makes this JD format genuinely useful as a filter. Generic culture statements ('we value teamwork and innovation') attract everyone and filter nobody. Specific statements ('we do not have weekly status meetings; we write everything down and you are expected to read it') attract the candidates who thrive in that environment and signal clearly to those who would not. The 30/90/180-day milestone format replaces aspirational role descriptions with accountable commitments.

---

## Sample Output

Culture Statement 3: We are a two-person team. There is no one to escalate to, no process to follow when something goes wrong, and no colleague to pick up your work if you need a week off. The person who succeeds here builds the safety nets as well as uses them.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
