# Market Gap and White Space Identifier

**Domain:** Market Research and Competitive Intelligence
**Level:** 🔴 Advanced

> Analyse competitor clustering, pricing gaps, underserved segments, and unoccupied feature territories to identify the white space a new entrant can own. Produces a defensible market entry position.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[MARKET_CATEGORY]` | The market you are entering | e.g. UK RegTech compliance monitoring software |
| `[KNOWN_PLAYERS]` | The major players in this market | e.g. ComplyAdvantage, Clausematch, Ascent RegTech, Encompass, manual processes |
| `[YOUR_CAPABILITIES]` | What you can build, deliver, or do that others cannot or have not | e.g. UK-specific regulatory training data, FCA handbook integration, CCO-led design process |
| `[CUSTOMER_SEGMENTS_UNDERSERVED]` | Any segments you believe are currently underserved | e.g. Mid-market financial services firms (50-500 staff), too large for manual processes, too small for enterprise RegTech |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a market strategy and competitive positioning expert with 20 years of experience identifying white space in crowded markets. You have helped over 30 companies find and occupy defensible positions in markets where the obvious spaces appeared to already be taken.
</role>

<context>
Market category: [MARKET_CATEGORY]
Known players: [KNOWN_PLAYERS]
Your capabilities: [YOUR_CAPABILITIES]
Potentially underserved segments: [CUSTOMER_SEGMENTS_UNDERSERVED]
</context>

<instructions>
Think through this step by step before producing output.

Step 1: Map the competitive clustering. Where are most competitors positioned on two axes: (a) Product Complexity (Simple to Enterprise-grade) and (b) Customer Segment (SME to Large Enterprise)? Identify the quadrants that are crowded and the quadrants that are underserved.

Step 2: Identify pricing gaps. What price points are currently unserved in this market? Is there a gap between free/low-cost tools and enterprise pricing that a mid-market product could occupy?

Step 3: Identify feature territory gaps. What capabilities do customers need that no current player adequately provides? Cross-reference with the capabilities stated in the inputs.

Step 4: Identify the underserved segment opportunity. Score each stated underserved segment across: Segment Size, Urgency of Need, Current Solution Quality, and Accessibility. Identify the highest-scoring segment.

Step 5: Define the white space position. Articulate the specific combination of segment, price point, and feature territory that is currently unoccupied and aligns with your capabilities.
</instructions>

<output_format>
Section 1: Competitive Clustering Map Description: a 2x2 matrix description (written, not drawn) identifying which quadrants are crowded, contested, and empty.
Section 2: Pricing Gap Analysis: table with Price Band, Current Players, Gap Assessment (Crowded/Contested/Empty) columns.
Section 3: Feature Territory Gaps: table with Feature Territory, Current Provision Quality (1-5), Importance to Target Customer (1-5), and Gap Score columns.
Section 4: Underserved Segment Scoring: table with Segment, Size Score, Urgency Score, Solution Quality Score, Accessibility Score, and Total columns.
Section 5: White Space Definition: one precise paragraph defining the specific position available, why it is defensible, and why your capabilities align with it.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- The 2x2 description must be specific about which named players sit in which quadrants.
- Pricing gap analysis must use real or realistic price bands for this market, not invented ranges.
- Feature territory gaps must be specific to the market category, not generic software gaps.
- The white space definition must be a specific, occupiable position, not a general statement about serving underserved customers.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Named players are placed in specific quadrants with rationale.
2. Pricing bands are realistic for this market category.
3. Feature territory gaps are specific to compliance/regulatory technology, not generic.
4. Segment scores are differentiated, not all segments scored the same.
5. White space definition names a specific position that combines segment, price, and feature territory.
</evaluation_criteria>
```

---

## Why This Works

White space identification fails when it is done as a purely theoretical exercise. Anchoring the analysis in competitive clustering, pricing reality, and capability alignment produces positions that are both available and winnable. The scoring matrix for underserved segments prevents founders from selecting the largest or most exciting segment rather than the most accessible one.

---

## Sample Output

Feature Territory Gap row: FCA-specific obligation mapping | 2 | 5 | Gap Score: 10, highest priority white space; no current player has trained on the full FCA handbook with UK employment law overlay

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
