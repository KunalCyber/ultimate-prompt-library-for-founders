# Launch Playbook and Checklist Builder

**Domain:** Go-to-Market and Launch
**Level:** 🔵 Practitioner

> Build a phased launch playbook with pre-launch, launch day, and post-launch phases. Every action has an owner, a deadline, and a success criterion. No launch surprises.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you are launching | e.g. Version 1.0 of ComplianceOS, AI compliance monitoring SaaS |
| `[LAUNCH_DATE]` | Target launch date | e.g. 14 April 2025 |
| `[TARGET_AUDIENCE]` | Who you want to reach at launch | e.g. CCOs and compliance managers at UK financial services firms, LinkedIn audience of 800, existing waitlist of 45 contacts |
| `[LAUNCH_GOALS]` | What success looks like at 30 days post-launch | e.g. 3 paying customers, 20 demo requests, 500 LinkedIn impressions on launch post, coverage in one industry publication |
| `[TEAM_AVAILABLE]` | Who is available to execute the launch | e.g. 2 co-founders (1 technical, 1 commercial), no marketing hire, £2,000 launch budget |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a product launch strategist with 15 years of experience planning and executing B2B SaaS launches from private beta through general availability. You have run launches that generated 500 demo requests in 48 hours and post-mortemed launches that generated three. You know the difference between them.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
Launch date: [LAUNCH_DATE]
Target audience: [TARGET_AUDIENCE]
Launch goals: [LAUNCH_GOALS]
Team available: [TEAM_AVAILABLE]
</context>

<instructions>
Step 1: Define the launch phases: Pre-Launch (T-30 to T-1), Launch Day (T), and Post-Launch (T+1 to T+30). For each phase, identify the primary objective.

Step 2: Build the pre-launch checklist. Every action must have: the task, the owner role, the deadline relative to launch date, and the definition of done.

Step 3: Build the launch day checklist. Hour-by-hour if needed. Every action with owner and timing.

Step 4: Build the post-launch checklist covering the first 30 days. Focus on converting launch attention into pipeline and paying customers.

Step 5: Identify the three highest-risk failure points in this launch and the mitigation for each.
</instructions>

<output_format>
Section 1: Launch Phase Objectives. Three rows (Pre-Launch / Launch Day / Post-Launch) with Phase, Duration, Primary Objective, and Success Criterion columns.
Section 2: Pre-Launch Checklist. Table with Task, Owner, Deadline (T-X days), Definition of Done, and Status (leave blank) columns. Organised by category: Product, Content, Outreach, Technical.
Section 3: Launch Day Checklist. Table with Time, Task, Owner, and Done columns. Hour-by-hour for key moments.
Section 4: Post-Launch Checklist (T+1 to T+30). Table with Week, Task, Owner, and Goal columns.
Section 5: Risk and Mitigation. Three numbered risks with Failure Point, Probability (H/M/L), Impact (H/M/L), and Mitigation columns.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Every checklist item must have a specific owner role and deadline. No orphaned tasks.
- Definition of done must be observable and binary: either done or not done.
- Post-launch checklist must focus on conversion, not continuation of launch activities.
- Risk mitigations must be specific pre-emptive actions, not contingency plans activated after the failure occurs.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every checklist item has an owner and a deadline.
2. Definition of done is observable and binary for every pre-launch item.
3. Launch day checklist has hour-by-hour timing for key activities.
4. Post-launch checklist focuses on pipeline conversion, not vanity metrics.
5. Risk mitigations are pre-emptive, not reactive.
</evaluation_criteria>
```

---

## Why This Works

The definition of done column is what separates a launch checklist from a launch wish list. Most launch plans contain tasks with no clear completion criterion, which means they exist in a permanent state of partial progress. The hour-by-hour launch day structure forces founders to confront resource constraints before launch day, not during it.

---

## Sample Output

Pre-Launch item: LinkedIn launch post drafted and approved | Owner: Commercial Co-founder | Deadline: T-7 | Definition of Done: Post is written, reviewed by both founders, contains product screenshot or demo clip, CTA links to working landing page, and scheduled for 8:00 AM on launch day

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
