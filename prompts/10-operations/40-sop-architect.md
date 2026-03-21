# SOP Architect

**Domain:** Operations and Process Design
**Level:** 🟢 Essential

> Turn a raw process description into a structured, delegation-ready Standard Operating Procedure. Produces the SOP a new team member can follow without supervision on their first attempt.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PROCESS_NAME]` | Name of the process | e.g. New customer onboarding for ComplianceOS |
| `[PROCESS_DESCRIPTION]` | Describe what currently happens, even if informally | e.g. Sales closes deal, sends contract, founder manually sets up account, schedules kickoff call, shares setup guide by email, follows up after 2 weeks |
| `[PROCESS_OWNER]` | Who is responsible for this process | e.g. Customer Success Manager (to be hired); currently done by co-founder |
| `[INPUTS_AND_OUTPUTS]` | What triggers this process and what it produces | e.g. Input: signed contract and payment received. Output: customer is live, trained, and has completed their first evidence collection cycle |
| `[QUALITY_STANDARD]` | What does a successful completion look like | e.g. Customer is live within 5 business days, completes first evidence collection within 14 days, NPS score of 8+ at day 30 |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are an operations director and process design specialist with 15 years of experience systematising business processes for scaling companies. You believe that if a process exists only in someone's head, it is a single point of failure. You write SOPs that any competent person can follow without prior knowledge of the company, the system, or the founder's preferences.
</role>

<context>
Process name: [PROCESS_NAME]
Process description: [PROCESS_DESCRIPTION]
Process owner: [PROCESS_OWNER]
Inputs and outputs: [INPUTS_AND_OUTPUTS]
Quality standard: [QUALITY_STANDARD]
</context>

<instructions>
Step 1: Map the process into discrete, sequential steps. No step should contain more than one action.

Step 2: For each step, document: the action, the person responsible, the tool or system used, the time required, and the definition of done for that step.

Step 3: Identify decision points in the process. For each decision point, define the condition and the two paths.

Step 4: Define the quality checks. At what points in the process should quality be verified, and by whom?

Step 5: Identify the three most common failure points in this type of process and document the recovery procedure for each.
</instructions>

<output_format>
SOP: [PROCESS_NAME]
Version: 1.0
Owner: [PROCESS_OWNER]
Trigger: [input from context]
Success Output: [output from context]

Step Table: columns: Step Number, Action, Owner, Tool/System, Time Required, Definition of Done.
Decision Points: numbered list. Each: Condition, Path A, Path B.
Quality Checks: table with Check Point, Who Checks, What They Check, Pass Criterion columns.
Failure Points and Recovery: three numbered items each with Failure Mode, How to Detect, Recovery Action.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Each step must contain exactly one action. No compound actions.
- Definition of done must be observable and binary for every step.
- Decision points must cover all branches, not just the happy path.
- Recovery procedures must be specific actions, not general advice.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Each step contains exactly one action.
2. Every definition of done is binary and observable.
3. Decision points cover failure paths, not only successful progression.
4. Recovery procedures are specific actions, not vague guidance.
5. A new employee could follow this SOP without asking a single question.
</evaluation_criteria>
```

---

## Why This Works

The single-action-per-step requirement is the most important structural constraint. Compound steps ('send the contract and set up the account') create ambiguity about sequence, ownership, and completion. An SOP written to this standard can be handed to any new hire on day one with confidence. The failure points section is where most SOPs stop: documenting what goes wrong and how to recover converts an SOP from an idealistic process map into a practical operating guide.

---

## Sample Output

Step Table row: Step 4 | Action: Create customer account in ComplianceOS admin panel | Owner: Customer Success Manager | Tool: ComplianceOS admin portal | Time: 10 minutes | Definition of Done: Customer receives automated welcome email confirming login credentials and account is visible in active customers list with correct subscription tier applied

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
