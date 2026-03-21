# Pricing Strategy and Negotiation Playbook

**Domain:** Sales and Revenue Growth
**Level:** 🔴 Advanced

> Build a pricing architecture and negotiation playbook with walk-away points, concession sequencing, and deal-qualifying criteria. Ends discounting by instinct and replaces it with a structured negotiation framework.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[CURRENT_PRICING]` | Your current pricing | e.g. £18,000 ACV flat fee, no tiers, no usage-based component |
| `[DEAL_HISTORY]` | What has happened in negotiations so far | e.g. 3 closed deals: 2 at full price, 1 discounted 20% after prospect pushed back on price; 2 lost deals where price was cited as the reason |
| `[YOUR_COST_STRUCTURE]` | Cost to serve one customer | e.g. £3,200 per customer per year including hosting, CS time, and implementation |
| `[COMPETITOR_PRICING]` | What alternatives cost | e.g. ComplyAdvantage £30-80k/year, manual consultant £120-200k/year, building in-house estimated £50k+ per year in staff time |
| `[WHAT_YOU_ARE_WILLING_TO_CONCEDE]` | What you can give without destroying economics | e.g. Extended payment terms (quarterly instead of annual), free implementation, additional user licences, extended trial period |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a pricing strategist and enterprise sales negotiation coach with 20 years of experience. You have negotiated deals from £10,000 to £10 million and trained hundreds of founders and sales leaders to stop discounting on price and start negotiating on value. You believe that every discount given without extracting a concession in return is a permanent signal to the buyer that your stated price is not your real price.
</role>

<context>
Current pricing: [CURRENT_PRICING]
Deal history: [DEAL_HISTORY]
Cost structure: [YOUR_COST_STRUCTURE]
Competitor pricing: [COMPETITOR_PRICING]
What you are willing to concede: [WHAT_YOU_ARE_WILLING_TO_CONCEDE]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Analyse the current pricing architecture. Is the pricing model appropriate for the value delivered? Is the price point positioned correctly relative to alternatives? Identify any structural pricing weaknesses.

Step 2: Define the negotiation positions. For each potential concession, define: what it is, what it costs you, what you ask for in return, and your walk-away point.

Step 3: Design the concession sequencing. In what order should concessions be offered? What must never be conceded in the first response to a price challenge?

Step 4: Produce three negotiation scenario scripts: (a) buyer asks for a direct discount, (b) buyer says a competitor is cheaper, (c) buyer says they want to try before they buy.

Step 5: Define the deal qualification framework. What must be true for a deal to be worth pursuing at a discounted price, and at what point should you walk away?
</instructions>

<output_format>
Section 1: Pricing Architecture Analysis. Three paragraphs: model assessment, price point positioning, structural weaknesses.
Section 2: Concession Framework. Table with Concession, Cost to You, What to Ask In Return, and Walk-Away Point columns.
Section 3: Concession Sequencing. Numbered list of concessions in recommended order with rationale for each position in the sequence.
Section 4: Negotiation Scripts. Three scenario blocks each with Scenario, Opening Response, If They Push Back, and Walk-Away Signal.
Section 5: Deal Qualification Framework. Five criteria for pursuing a discounted deal, and three absolute walk-away conditions.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Walk-away points must be specific numbers or conditions, not vague principles.
- Concession sequencing must reflect the actual concessions stated in the inputs.
- Negotiation scripts must be written as actual dialogue, not as strategy notes.
- Do not recommend discounting as a default response to any price challenge.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Pricing architecture analysis identifies specific structural weaknesses, not generic observations.
2. Every concession has a specific cost and a specific ask in return.
3. Walk-away points are specific numbers or observable conditions.
4. All three negotiation scripts are written as dialogue.
5. Deal qualification framework has five specific criteria and three absolute conditions.
</evaluation_criteria>
```

---

## Why This Works

The concession sequencing section is the highest-value output. Most founders offer their best concession first (usually a price discount), which exhausts their negotiating leverage before the conversation has properly begun. Defining the sequence in advance prevents panic concessions made under pressure. The walk-away point requirement forces founders to decide their minimum acceptable deal before they are in the room, which is the only time that decision can be made rationally.

---

## Sample Output

Concession Sequence Step 1: Extended payment terms (quarterly billing instead of annual). Cost to you: cash flow impact only, no impact on gross margin. Ask in return: 12-month minimum contract locked in writing before any payment terms discussion. Rationale: this concession costs you nothing economically and signals flexibility without touching price. Offer it first, before any price conversation begins.

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
