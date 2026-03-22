# Interview Scorecard and Hiring Rubric Builder

**Domain:** People, Culture and Hiring
**Level:** 🔵 Practitioner

> Build a structured interview process with scorecards, evaluation criteria, interview questions, and red flag indicators. Replaces vibes-based hiring with a repeatable, defensible process.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[ROLE_TITLE]` | The role you are hiring for | e.g. Head of Customer Success |
| `[CRITICAL_COMPETENCIES]` | The 4-5 competencies that matter most for success in this role | e.g. (1) Customer relationship depth, (2) Process design from scratch, (3) Data-driven retention management, (4) Communication under pressure, (5) Commercial awareness |
| `[INTERVIEW_STAGES]` | How many stages and who is involved | e.g. Stage 1: 30-min screening call (founder). Stage 2: 60-min competency interview (both founders). Stage 3: 30-min case study presentation. Stage 4: reference calls |
| `[NON_NEGOTIABLE_VALUES]` | Values or working styles that are absolute requirements | e.g. Radical transparency about problems, ownership without being told, written-first communication |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a hiring process designer and talent assessment specialist with 15 years of experience building structured interview processes for high-stakes roles at scaling companies. You have seen the cost of a bad hire at an early-stage company, and you know that structured interviews with consistent scoring criteria outperform unstructured interviews at every stage of growth.
</role>

<context>
Role title: [ROLE_TITLE]
Critical competencies: [CRITICAL_COMPETENCIES]
Interview stages: [INTERVIEW_STAGES]
Non-negotiable values: [NON_NEGOTIABLE_VALUES]
</context>

<instructions>
Step 1: Design the interview structure. For each stage, define the objective, the competencies assessed, and who conducts it.

Step 2: Write two behavioural interview questions per competency. Each question must use the STAR format (Situation, Task, Action, Result) and target a specific experience the candidate should be able to describe.

Step 3: Define the scoring rubric for each competency. For each, describe what a 1, 3, and 5 score looks like in observable, specific terms.

Step 4: Design the red flag indicator list. What specific answers, behaviours, or signals in the interview should trigger a No regardless of other scores?

Step 5: Produce the scorecard template. A single document an interviewer completes immediately after each stage.
</instructions>

<output_format>
Section 1: Interview Structure. Table with Stage, Objective, Competencies Assessed, Interviewer, and Duration columns.
Section 2: Question Bank. One block per competency with two STAR-format questions and the follow-up probe for each.
Section 3: Scoring Rubric. One block per competency with Score 1 (description), Score 3 (description), Score 5 (description).
Section 4: Red Flag Indicators. Numbered list of specific red flags with the concern each signals.
Section 5: Scorecard Template. Formatted as a usable document: candidate name, date, stage, competency scores, red flags noted, overall recommendation (Strong Yes / Yes / No / Strong No), and one-paragraph justification field.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Scoring rubric descriptions must be observable and specific, not adjective-based.
- Red flags must be specific behaviours or answers, not vague concerns.
- Questions must target the stated competencies, not generic interview questions.
- Scorecard must be completable in under 10 minutes immediately after the interview.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every question targets a specific stated competency.
2. Scoring rubric uses observable behaviours, not adjectives.
3. Red flags are specific enough to trigger a consistent response across different interviewers.
4. Scorecard is completable in under 10 minutes.
5. Strong Yes / Yes / No / Strong No recommendation is required, not optional.
</evaluation_criteria>
```

---

## Why This Works

The observable scoring rubric is the mechanism that makes structured interviewing actually work. A rubric that says '5 = excellent communication' is not a rubric: it is an invitation for each interviewer to apply their own definition of excellent. A rubric that says '5 = candidate described a situation where they identified a client at churn risk before it was flagged, took autonomous action, and documented the intervention for the team' produces consistent scores across interviewers and reduces the influence of personal rapport on hiring decisions.

---

## Sample Output

Red Flag 2: When asked about a failure or a difficult customer situation, candidate describes the failure as primarily caused by their organisation, their manager, or their tools, with no acknowledgement of what they personally could have done differently. Concern: signals low ownership and a pattern of externalising responsibility that will manifest as a problem in a startup environment with limited process and support.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
