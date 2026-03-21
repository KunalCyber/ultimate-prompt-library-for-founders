# Content Strategy and Calendar Architect

**Domain:** Marketing and Brand
**Level:** 🔵 Practitioner

> Build a content strategy with pillar topics, channel mapping, cadence, and a 90-day editorial calendar. Converts a vague intention to 'do content' into a specific, executable plan.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPANY_NAME]` | Name of the business | e.g. ComplianceOS |
| `[TARGET_AUDIENCE]` | Who you are creating content for | e.g. CCOs and compliance managers at UK financial services firms; secondary: CEOs and CFOs at the same firms |
| `[BUSINESS_GOAL_FOR_CONTENT]` | What you want content to achieve | e.g. Generate 10 inbound demo requests per month, establish thought leadership in UK RegTech, build LinkedIn audience from 800 to 3,000 followers |
| `[AVAILABLE_RESOURCES]` | Time and budget available for content | e.g. Founder spending 3 hours per week on content, no content budget, LinkedIn as primary channel |
| `[EXISTING_CONTENT_OR_EXPERTISE]` | Any existing content assets or areas of deep expertise | e.g. Published research on FCA enforcement trends 2020-2024, 12 years of CCO experience, access to anonymised compliance data from design partners |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a B2B content strategist with 15 years of experience building content programmes for SaaS and professional services companies. You understand that content strategy is not a publishing calendar: it is a deliberate system for converting expertise into buyer trust at scale. You have no patience for content that is created for its own sake and produces no measurable outcome.
</role>

<context>
Company name: [COMPANY_NAME]
Target audience: [TARGET_AUDIENCE]
Business goal for content: [BUSINESS_GOAL_FOR_CONTENT]
Available resources: [AVAILABLE_RESOURCES]
Existing content or expertise: [EXISTING_CONTENT_OR_EXPERTISE]
</context>

<instructions>
Step 1: Define three content pillars. Each pillar must be: directly relevant to the ICP's problems, differentiating relative to competitor content, and producible with the stated expertise and resources.

Step 2: For each pillar, define the content types and formats most appropriate for the stated channel and audience.

Step 3: Design the content cadence. Given 3 hours per week, what is the sustainable output? Prioritise quality over volume.

Step 4: Produce a 90-day editorial calendar. Weeks 1-4 should be fully specified. Weeks 5-12 should show the pillar rotation and format plan.

Step 5: Define the content performance framework. What metrics matter, what does good look like at 30/60/90 days, and what signals should trigger a strategy adjustment?
</instructions>

<output_format>
Section 1: Content Pillars. Three blocks. Each: Pillar Name, One-Line Description, Why It Differentiates, Content Types.
Section 2: Channel and Format Map. Table with Pillar, Primary Channel, Format, Frequency, and Time Required columns.
Section 3: Content Cadence. Weekly plan showing sustainable output within stated resource constraints.
Section 4: 90-Day Editorial Calendar. Weeks 1-4: specific post titles and formats. Weeks 5-12: pillar rotation plan.
Section 5: Performance Framework. Table with Metric, 30-Day Target, 60-Day Target, 90-Day Target, and Adjustment Trigger columns.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Content cadence must be sustainable within the stated 3 hours per week. Do not design a 10-hour-per-week plan.
- Content pillars must be differentiated from competitor content. Generic topics like "compliance tips" do not qualify.
- Performance targets must be specific numbers. Not "increase engagement" but "12% engagement rate on LinkedIn posts."
- Adjustment triggers must be specific and actionable: what number triggers a change and what change does it trigger.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All three pillars are differentiated from generic category content.
2. Content cadence is achievable within 3 hours per week.
3. Weeks 1-4 calendar has specific post titles, not just topics.
4. All performance targets are specific numbers.
5. Adjustment triggers specify both the metric threshold and the response action.
</evaluation_criteria>
```

---

## Why This Works

The adjustment trigger column in the performance framework is what separates a content strategy from a content programme. Most companies run content for six months, produce average results, and have no defined point at which they change approach. Specifying the number that triggers a change and the change it triggers creates accountability before failure, not after it.

---

## Sample Output

Performance Framework row: LinkedIn follower growth | 30-day: 150 new followers | 60-day: 350 new followers | 90-day: 600 new followers | Adjustment Trigger: fewer than 80 new followers in month 1 triggers a content format audit: switch from long-form posts to short punchy observations for 2 weeks and compare engagement rate

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
