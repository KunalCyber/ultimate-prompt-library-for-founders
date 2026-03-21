# Go-to-Market Strategy and Channel-Market Fit Analyser

**Domain:** Go-to-Market and Launch
**Level:** 🔴 Advanced

> Produce a complete GTM strategy covering channels, messaging, sequencing, resources, and success metrics. Moves from 'we will do sales and marketing' to a specific, sequenced GTM motion with channel-market fit analysis.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[PRODUCT_OR_SERVICE]` | What you sell | e.g. AI compliance monitoring SaaS for UK financial services |
| `[ICP]` | Your defined ideal customer profile | e.g. CCOs at FCA-regulated financial services firms, 50-500 employees, annual compliance budget above £100k |
| `[CURRENT_RESOURCES]` | Sales and marketing headcount and budget available | e.g. 1 founder doing sales, £3,000/month marketing budget, no dedicated marketing hire for 6 months |
| `[CURRENT_TRACTION]` | Any existing proof of channel performance | e.g. 2 customers acquired via founder network, 1 via LinkedIn outreach, 0 via inbound, 3 pending referrals from design partners |
| `[SALES_CYCLE_LENGTH]` | Observed or estimated sales cycle | e.g. 45 days average from first meeting to signed contract based on 3 closed deals |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a GTM strategist with 20 years of experience designing and executing go-to-market motions for B2B SaaS companies from pre-revenue through Series B. You have seen every GTM mistake and know that the most common one is pursuing too many channels simultaneously with insufficient resources to make any of them work. You believe in channel-market fit: finding the one or two channels that work before scaling anything.
</role>

<context>
Product or service: [PRODUCT_OR_SERVICE]
ICP: [ICP]
Current resources: [CURRENT_RESOURCES]
Current traction: [CURRENT_TRACTION]
Sales cycle length: [SALES_CYCLE_LENGTH]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Evaluate channel-market fit for six potential GTM channels: founder-led outbound, content and SEO, LinkedIn outbound, events and conferences, partner and channel sales, and product-led growth. Score each on: ICP Reachability (can this channel reach the stated ICP?), Resource Fit (can this be executed with stated resources?), and Signal from Traction (what does existing traction tell us about this channel?).

Step 2: Identify the primary channel and the secondary channel. The primary channel must be the one with the highest product of ICP reachability and resource fit, anchored by any traction signal available.

Step 3: Design the primary channel motion in detail: specific tactics, weekly activity targets, conversion rate assumptions at each stage, and the first 30-day action plan.

Step 4: Define the channel success metrics. What does working look like at 30 days, 60 days, and 90 days? What does not working look like, and what is the trigger to switch?

Step 5: Identify the GTM sequencing. What comes first, what comes second, and what must not be started until the primary channel is proven?
</instructions>

<output_format>
Section 1: Channel-Market Fit Scoring. Table with Channel, ICP Reachability (1-5), Resource Fit (1-5), Traction Signal (1-5), Total, and Recommendation (Primary / Secondary / Defer) columns.
Section 2: Primary Channel Motion. Structured block with Tactic, Weekly Activity Target, Conversion Assumption, and Monthly Output columns.
Section 3: 30-Day Action Plan. Numbered list of specific weekly actions for weeks 1-4.
Section 4: Channel Success Metrics. Table with Timeframe (30/60/90 days), Working Signal, and Not Working Signal columns.
Section 5: GTM Sequencing. Three phases with start condition, activities, and exit criteria for each.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Channel scores must reflect the stated resources and ICP. A channel requiring £50k/month is not a 5 on Resource Fit for a £3k/month budget.
- Primary channel motion must be executable with stated headcount and budget.
- 30-day actions must be specific daily or weekly activities, not strategic goals.
- Not Working signals must be specific metrics, not vague statements.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All six channels are scored with rationale anchored in the stated resources and ICP.
2. Primary channel motion is executable within stated resource constraints.
3. 30-day actions are specific and weekly.
4. Success metrics include both Working and Not Working signals for all three timeframes.
5. GTM sequencing has specific start conditions and exit criteria.
</evaluation_criteria>
```

---

## Why This Works

Channel-market fit scoring prevents the most common GTM failure: spreading limited resources across five channels and achieving nothing on any of them. The Not Working signal in the success metrics section is the most commonly missing element in GTM plans. Without a defined point at which to stop and change, founders persist with failing channels until the runway runs out.

---

## Sample Output

Channel Success Metric row: 60 days | Working Signal: 3 qualified discovery calls per week from outbound, at least one advancing to pilot stage | Not Working Signal: Fewer than 1 qualified discovery call per week after 200 personalised outreach attempts, suggesting either ICP targeting or messaging is wrong, not volume

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
