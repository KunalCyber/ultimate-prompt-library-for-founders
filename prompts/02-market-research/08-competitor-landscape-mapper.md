# Competitor Landscape Mapper

**Domain:** Market Research and Competitive Intelligence
**Level:** 🔵 Practitioner

> Identify, profile, and compare competitors across positioning, pricing, strengths, weaknesses, and market share. Produce the competitive analysis a Series A investor would expect to see.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[YOUR_PRODUCT]` | What your product does and who it serves | e.g. AI compliance monitoring SaaS for UK-regulated financial services firms |
| `[YOUR_PRIMARY_DIFFERENTIATOR]` | The single strongest claim you make vs alternatives | e.g. UK regulatory training vs US-trained competitors; 94% accuracy on FCA-specific obligations |
| `[KNOWN_COMPETITORS]` | List any competitors you are already aware of | e.g. ComplyAdvantage, Ascent RegTech, Clausematch, manual spreadsheet processes, Big 4 advisory |
| `[CUSTOMER_SEGMENT]` | The specific customer you are targeting | e.g. CCOs at FCA-regulated financial services firms, 50-500 employees |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a competitive intelligence analyst and go-to-market strategist with 15 years of experience mapping competitive landscapes for B2B SaaS, marketplace, and professional services companies. You have produced competitive analyses for Series A through Series C fundraising processes.
</role>

<context>
Your product: [YOUR_PRODUCT]
Your primary differentiator: [YOUR_PRIMARY_DIFFERENTIATOR]
Known competitors: [KNOWN_COMPETITORS]
Customer segment: [CUSTOMER_SEGMENT]
</context>

<instructions>
Step 1: Identify the full competitive set. Include: direct competitors (same product, same customer), indirect competitors (different product, same problem), and status quo alternatives (how customers currently solve the problem without a dedicated tool). Add any relevant competitors not listed in the inputs.

Step 2: For each competitor, research and document: founding year, funding status (if known), pricing model, primary customer segment, key differentiator, and primary weakness.

Step 3: Score each competitor across five dimensions relevant to the stated customer segment: Product Depth, Pricing Accessibility, UK/Local Regulatory Fit, Sales Cycle Complexity, and Customer Support Quality. Score 1-5.

Step 4: Identify the two most dangerous competitors and explain specifically why they are dangerous.

Step 5: Define your competitive positioning statement: the specific space in the market you occupy that is currently underserved or contested.
</instructions>

<output_format>
Section 1: Competitive Landscape Overview: one paragraph categorising the competitive set.
Section 2: Competitor Profiles Table: one row per competitor. Columns: Name | Type (Direct/Indirect/Status Quo) | Funding | Pricing Model | Primary Customer | Key Differentiator | Primary Weakness.
Section 3: Competitive Scoring Matrix: competitors as rows, five dimensions as columns. Each cell: score (1-5). Final column: Total Score.
Section 4: Most Dangerous Competitors: two paragraphs, one per competitor, explaining the specific threat and how to counter it.
Section 5: Positioning Statement: one paragraph defining the specific space you occupy and why it is defensible.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Do not invent competitor details. If a funding amount or pricing model is unknown, state "not publicly disclosed."
- Competitive scores must reflect genuine differentiation. Do not score all competitors identically on any dimension.
- The positioning statement must be specific. "Better, faster, cheaper" is not a position.
- The two most dangerous competitors must be identified by name with specific threat analysis.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All three competitor types are represented (Direct, Indirect, Status Quo).
2. No invented competitor details, unknowns are marked as such.
3. Scoring matrix shows genuine differentiation across dimensions.
4. Most dangerous competitor analysis names specific threats, not generic competitive risks.
5. Positioning statement is specific and defensible.
</evaluation_criteria>
```

---

## Why This Works

Including status quo alternatives is the most commonly missed component of competitive analysis. The biggest competitor for most B2B products is not another software vendor, it is the spreadsheet, the consultant, or the manual process. Scoring across dimensions relevant to the specific customer segment produces insight that generic feature comparisons miss.

---

## Sample Output

Competitor Profile row: ComplyAdvantage | Direct | $88m raised (Series C) | Usage-based + platform fee | AML/KYC compliance teams at banks and fintechs | Real-time transaction monitoring | Does not address UK employment law or FCA conduct obligations, narrow use case

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
