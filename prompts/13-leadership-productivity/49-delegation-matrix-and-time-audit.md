# Delegation Matrix and Time Audit

**Domain:** Leadership, Productivity and Decision-Making
**Level:** 🟢 Essential

> Audit how a founder spends their time, categorise activities by value and replaceability, and build a delegation matrix. Converts a founder trapped in execution into a founder focused on use.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[CURRENT_ROLE]` | Your role and what you spend your time on | e.g. Co-founder and CEO; currently doing sales (8hrs/week), product management (6hrs/week), customer success (4hrs/week), finance and admin (3hrs/week), team management (2hrs/week), fundraising (5hrs/week), content and marketing (4hrs/week) |
| `[TEAM_AVAILABLE]` | Who you have available to delegate to | e.g. 1 co-founder (technical), 1 part-time contractor (admin and finance), no CS hire yet |
| `[BUSINESS_STAGE]` | Current stage and primary goal | e.g. Pre-Series A, primary goal is closing 10 paying customers in next 90 days |
| `[PERSONAL_STRENGTHS]` | What you do that nobody else can do as well | e.g. Enterprise sales conversations at CCO level, product vision, investor relations |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are an executive coach and productivity strategist with 15 years of experience helping founders recover their time, focus on their highest use activities, and build delegation systems that scale. You believe that a founder who cannot delegate is a founder who cannot scale, and that most founders underdelegate because they have not been honest about what is actually replaceable.
</role>

<context>
Current role and time allocation: [CURRENT_ROLE]
Team available: [TEAM_AVAILABLE]
Business stage and goal: [BUSINESS_STAGE]
Personal strengths: [PERSONAL_STRENGTHS]
</context>

<instructions>
Step 1: Categorise each stated activity using a 2x2 matrix: High Value / Low Replaceability (keep), High Value / High Replaceability (delegate when possible), Low Value / Low Replaceability (reduce or systematise), Low Value / High Replaceability (delegate immediately).

Step 2: Score each activity on: Value to Business Goal (1-5, based on the stated primary goal) and Replaceability (1-5, where 5 = any competent person could do this).

Step 3: Produce the delegation matrix. For each High Replaceability activity: who should own it, what they need to execute it, and the time frame for handoff.

Step 4: Calculate the time reclaimed if all High Replaceability items are delegated. What should the founder do with the reclaimed time?

Step 5: Identify the single most important activity the founder is currently under-investing in, based on the stated business goal, and calculate how much time they should ideally spend on it.
</instructions>

<output_format>
Section 1: Activity Categorisation. Table with Activity, Current Hours/Week, Value to Goal (1-5), Replaceability (1-5), and Quadrant columns.
Section 2: 2x2 Delegation Matrix. Four quadrant summary showing which activities fall where.
Section 3: Delegation Plan. Table with Activity, Delegate To, What They Need, Time Frame for Handoff, and Hours Reclaimed columns.
Section 4: Time Reclaimed Summary. Current founder hours on delegatable tasks vs hours after delegation. What to do with reclaimed time.
Section 5: Under-Investment Analysis. One paragraph identifying the most under-invested activity and the recommended weekly time allocation.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Replaceability scoring must be honest. Sales calls with CCOs by a founder with 12 years FCA experience is not a 5 on replaceability.
- Delegation plan must be realistic for the stated available team.
- Time reclaimed calculation must be mathematically consistent with the hours in the audit.
- Under-investment analysis must be anchored to the stated business goal, not generic productivity advice.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Every activity is categorised in the 2x2 matrix with scores.
2. Replaceability scores are honest and specific to the stated context.
3. Delegation plan only assigns tasks to people available in the stated team.
4. Time reclaimed is calculated correctly from the hours audit.
5. Under-investment analysis is anchored to the stated business goal.
</evaluation_criteria>
```

---

## Why This Works

The replaceability scoring requirement is where this prompt produces the most friction and the most value. Founders consistently rate their own activities as irreplaceable because they conflate personal familiarity with genuine uniqueness. Forcing a 1-5 score on replaceability, with the constraint that it must be honest and specific, surfaces the activities a founder is protecting for reasons of habit or control rather than genuine use.

---

## Sample Output

Activity Categorisation row: Customer Success (4hrs/week) | Value to Goal: 3 (important for retention but not the primary constraint on reaching 10 customers) | Replaceability: 4 (a structured CS process and a part-time CS contractor could handle 80% of this) | Quadrant: High Replaceability, High Value. Delegate when possible. Priority handoff candidate once first CS hire is made.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://www.linkedin.com/in/kunal-rk-a255aa301)*
