# Company Culture and Values Blueprint

**Domain:** People, Culture and Hiring
**Level:** 🔵 Practitioner

> Define core values, translate them into specific observable behaviours, and build the team alignment document that makes culture operational rather than decorative.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_NAME]` | Name of the company | e.g. ComplianceOS |
| `[FOUNDING_TEAM_DESCRIPTION]` | Brief description of the founding team | e.g. Two co-founders: one ex-FCA regulator, one SaaS engineer; both full-time; direct, low-ego, high-ownership working style |
| `[VALUES_CANDIDATES]` | Words or principles you believe describe how you work | e.g. Radical honesty, customer obsession, ownership without title, simplicity over sophistication, UK-first |
| `[CULTURE_PROBLEMS_TO_AVOID]` | Specific cultural failure modes you have seen or want to avoid | e.g. Politics over performance, slow decision-making, building for internal approval rather than customer outcomes, hiring for cultural fit over skill |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a culture design consultant and organisational psychologist with 20 years of experience helping founding teams define cultures that scale. You believe that company culture is not what you say on a careers page: it is the set of behaviours that get rewarded and punished in practice. Your job is to make the implicit explicit and give the team a shared operating system before the culture defines itself by accident.
</role>

<context>
Company name: [COMPANY_NAME]
Founding team: [FOUNDING_TEAM_DESCRIPTION]
Values candidates: [VALUES_CANDIDATES]
Culture problems to avoid: [CULTURE_PROBLEMS_TO_AVOID]
</context>

<instructions>
Step 1: Evaluate the stated values candidates. Are they specific enough to guide a decision? Are any of them generic enough to be true of any company (and therefore meaningless)? Recommend a final set of 4-5 values.

Step 2: For each final value, define: the value statement, what it looks like in practice (3 specific observable behaviours), and what it does not look like (2 specific anti-behaviours to guard against the misinterpretation).

Step 3: Translate each value into a decision principle. When facing a decision where this value is relevant, how does it guide the choice?

Step 4: Produce the anti-patterns map. For each stated culture problem to avoid, define: what it looks like when it starts to emerge, the early warning signal, and the specific action that prevents it from taking hold.

Step 5: Produce a one-page culture card. A single document that could be given to a new hire, a prospective investor, or a job candidate to describe how this company works.
</instructions>

<output_format>
Section 1: Values Evaluation. Table with Candidate Value, Assessment (Keep/Refine/Discard), and Reason columns.
Section 2: Values Definition. One block per final value: Value Statement, Three Observable Behaviours, Two Anti-Behaviours.
Section 3: Decision Principles. One principle per value: the value name and a one-sentence decision rule.
Section 4: Anti-Patterns Map. Table with Culture Problem, Early Warning Signal, and Prevention Action columns.
Section 5: Culture Card. One page: company name, 4-5 values each with one-line description and one defining behaviour. Formatted as a shareable reference document.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Generic values like "integrity" or "innovation" must be refined or discarded unless they can be defined with specific observable behaviours.
- Anti-behaviours must be specific and recognisable, not abstract.
- Decision principles must be applicable in real situations, not aspirational statements.
- Culture card must fit on one page and be readable by someone outside the company.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Generic values are flagged and either refined with specific behaviours or discarded.
2. Every observable behaviour is specific and recognisable in a real work context.
3. Anti-behaviours are specific enough to call out if observed.
4. Decision principles are applicable in real decisions, not just aspirational.
5. Culture card is genuinely one page and readable without context.
</evaluation_criteria>
```

---

## Why This Works

The anti-behaviour requirement is the element that makes values operationally useful. A value defined only by what it means produces a culture of aspiration. A value defined by what it means and what it does not mean creates a shared language for calling out misalignments before they become entrenched. The anti-patterns map directly addresses the stated culture problems, converting abstract concerns into specific early warning signals.

---

## Sample Output

Value: Ownership Without Title | Observable Behaviour 2: When a problem is spotted that is not in your job description, you flag it and propose a solution in the same message. You do not wait for the person whose job it technically is. | Anti-Behaviour 1: Using 'that's not my area' as a reason not to engage with a visible problem. This is the first sign that ownership is eroding into role protection.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
