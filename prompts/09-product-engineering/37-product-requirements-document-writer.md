# Product Requirements Document Writer

**Domain:** Product and Engineering
**Level:** 🔵 Practitioner

> Write a complete PRD covering problem statement, user stories, acceptance criteria, success metrics, dependencies, and explicit boundaries. Produces the document an engineering team can build from without follow-up questions.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_FEATURE]` | What you are building | e.g. Automated evidence collection module for FCA compliance monitoring platform |
| `[PROBLEM_BEING_SOLVED]` | The specific problem this solves | e.g. CCOs spend 3 days per quarter manually collecting compliance evidence from 6 internal systems |
| `[TARGET_USER]` | Who will use this feature | e.g. Chief Compliance Officer and compliance manager at FCA-regulated financial services firm |
| `[SUCCESS_DEFINITION]` | What does success look like when this ships | e.g. Evidence collection time reduced to under 2 hours, zero manual data entry, evidence audit trail complete |
| `[KNOWN_CONSTRAINTS]` | Technical, legal, or business constraints | e.g. Must integrate with existing FCA handbook API, must not store PII outside UK, must ship within 8 weeks |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a senior product manager with 15 years of experience writing PRDs for B2B SaaS products from 0-to-1 through to scaled engineering teams. You write PRDs that engineers can build from without follow-up questions and that stakeholders can evaluate without a walkthrough.
</role>

<context>
Product or feature: [PRODUCT_OR_FEATURE]
Problem being solved: [PROBLEM_BEING_SOLVED]
Target user: [TARGET_USER]
Success definition: [SUCCESS_DEFINITION]
Known constraints: [KNOWN_CONSTRAINTS]
</context>

<instructions>
Step 1: Write the problem statement. Two paragraphs: the current state without this feature, and the cost of that current state (time, money, risk, or user frustration).

Step 2: Define user stories. Write 4-6 user stories in the format: As a [role], I want to [action], so that [outcome]. Each must be specific and independently testable.

Step 3: Write acceptance criteria for each user story. Each criterion must be binary: either met or not met. No ambiguous success states.

Step 4: Define the success metrics. Three to five specific, measurable outcomes that confirm the feature delivered its intended value.

Step 5: Document dependencies and risks. What must exist or be completed before this can be built? What could prevent on-time delivery?

Step 6: Define explicit out-of-scope boundaries. What is deliberately not included in this version and why.
</instructions>

<output_format>
PRD: [PRODUCT_OR_FEATURE]

1. Problem Statement: two paragraphs.
2. User Stories: numbered list of 4-6 stories.
3. Acceptance Criteria: one block per user story with numbered criteria.
4. Success Metrics: numbered list of 3-5 metrics, each with a specific measurable target.
5. Dependencies and Risks: two tables. Dependencies: Dependency, Owner, Required By. Risks: Risk, Likelihood (H/M/L), Impact (H/M/L), Mitigation.
6. Out of Scope: numbered list with one-line rationale per item.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every acceptance criterion must be binary and testable by a QA engineer without interpretation.
- Success metrics must have specific numeric targets, not directional goals.
- Out of scope items must have a rationale, not just a list.
- No placeholder content. Every section must be specific to the stated product and problem.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every user story follows the As/Want/So That format and is independently testable.
2. Every acceptance criterion is binary and unambiguous.
3. All success metrics have specific numeric targets.
4. Dependencies table includes owner and required-by date or milestone.
5. Out of scope items each have a one-line rationale.
</evaluation_criteria>
```

---

## Why This Works

The binary acceptance criteria requirement is the most commercially valuable constraint. Acceptance criteria that contain words like 'easily', 'quickly', or 'appropriately' are not criteria: they are aspirations. The out-of-scope rationale requirement prevents scope creep in the next sprint by documenting the deliberate decision, not just the absence of a feature.

---

## Sample Output

User Story 2: As a compliance manager, I want the system to automatically retrieve evidence from our SharePoint, Jira, and email audit trail, so that I do not need to log into each system manually. Acceptance Criteria: (1) System connects to SharePoint via OAuth without requiring IT intervention. (2) Evidence retrieval completes within 4 minutes for a standard quarterly review set. (3) System surfaces a clear error message if a source system is unavailable, with the specific system named.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
