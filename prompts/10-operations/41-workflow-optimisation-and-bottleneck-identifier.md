# Workflow Optimisation and Bottleneck Identifier

**Domain:** Operations and Process Design
**Level:** 🔵 Practitioner

> Map a workflow, identify bottlenecks, and produce improvement recommendations with effort-impact scoring. Converts a frustrating operational problem into a prioritised action plan.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[WORKFLOW_NAME]` | Name of the workflow to analyse | e.g. Sales-to-cash workflow: from signed contract to first invoice paid |
| `[CURRENT_STEPS]` | Describe the current workflow steps in order | e.g. (1) Contract signed, (2) Finance notified by email, (3) Finance creates invoice manually in Xero, (4) Invoice emailed to customer, (5) Customer pays, (6) Revenue recognised in reporting, (7) Account activated in product |
| `[KNOWN_PROBLEMS]` | Issues you have already noticed | e.g. Step 3 takes 3-5 days due to finance team backlog; Step 7 is manual and occasionally forgotten; average time from signed contract to active account is 8 days |
| `[DESIRED_OUTCOME]` | What good looks like | e.g. Signed contract to active account in under 24 hours; zero manual steps; zero instances of delayed activation |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are an operations consultant and workflow analyst with 15 years of experience optimising business processes for scaling companies. You approach workflows as systems: every delay, error, and inefficiency has a root cause, and the root cause is almost always a handoff, a manual step, or an undefined ownership boundary.
</role>

<context>
Workflow name: [WORKFLOW_NAME]
Current steps: [CURRENT_STEPS]
Known problems: [KNOWN_PROBLEMS]
Desired outcome: [DESIRED_OUTCOME]
</context>

<instructions>
Step 1: Map the current workflow. For each step, document: the action, the owner, the average time taken, whether it is manual or automated, and the handoff point to the next step.

Step 2: Identify all bottlenecks. A bottleneck is any step where: work accumulates, delays propagate downstream, or errors are generated. Score each bottleneck by severity (impact on the desired outcome).

Step 3: Identify root causes. For each bottleneck, diagnose whether the cause is a process issue, a tool issue, an ownership issue, or a capacity issue.

Step 4: Produce improvement recommendations. For each bottleneck, suggest: the improvement, the effort required to implement (H/M/L), the impact on the desired outcome (H/M/L), and the implementation approach.

Step 5: Produce an optimised workflow. Show what the process looks like after all High Impact / Low-Medium Effort improvements are implemented.
</instructions>

<output_format>
Section 1: Current Workflow Map. Table with Step, Owner, Average Time, Manual or Automated, and Handoff Risk (H/M/L) columns.
Section 2: Bottleneck Analysis. Table with Step, Bottleneck Description, Severity (H/M/L), and Root Cause Type columns.
Section 3: Improvement Recommendations. Table with Bottleneck Step, Improvement, Effort (H/M/L), Impact (H/M/L), and Implementation Approach columns.
Section 4: Optimised Workflow. Table showing the improved process with projected time per step and total cycle time.
Section 5: Expected Outcome. One paragraph comparing current state to projected state with specific metrics.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Bottleneck severity must be assessed against the stated desired outcome, not in isolation.
- Root cause types must be specific: process, tool, ownership, or capacity. Not "inefficiency."
- Improvement recommendations must address root causes, not symptoms.
- Optimised workflow must be realistic: do not automate steps that require human judgment.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every step in the current workflow has an owner and time estimate.
2. Bottleneck severity is assessed against the stated desired outcome.
3. Root causes are classified into one of four specific types.
4. Improvements address root causes, not surface symptoms.
5. Optimised workflow shows a realistic projected cycle time.
</evaluation_criteria>
```

---

## Why This Works

The root cause classification requirement prevents the most common optimisation failure: recommending faster execution of a broken process. Classifying whether the cause is a process, tool, ownership, or capacity issue determines the correct type of intervention. A capacity bottleneck requires a hire or a reallocation; a tool bottleneck requires an integration or automation; they need completely different solutions.

---

## Sample Output

Bottleneck row: Step 3 (Finance creates invoice manually) | Bottleneck: 3-5 day delay due to finance team processing backlog | Severity: High (directly causes 8-day activation delay; damages first impression) | Root Cause: Tool issue. Xero invoice creation is manual because there is no integration between CRM and finance system. Automation would eliminate this step entirely.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
