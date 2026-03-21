# Competitor Review Pain-Point Miner

**Domain:** Market Research and Competitive Intelligence
**Level:** 🔵 Practitioner

> Extract unmet customer frustrations from competitor reviews and public feedback. Identify the gaps your product should fill and the messaging angles that will resonate with customers who have already tried the alternatives.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[COMPETITORS_TO_ANALYSE]` | Names of 2-4 competitors whose reviews you want to mine | e.g. ComplyAdvantage, Clausematch, Ascent RegTech |
| `[REVIEW_SOURCES]` | Where reviews exist (G2, Capterra, Trustpilot, App Store, LinkedIn comments) | e.g. G2, Capterra, LinkedIn posts from compliance professionals |
| `[YOUR_PRODUCT_CATEGORY]` | The category of product being reviewed | e.g. RegTech compliance monitoring software |
| `[TARGET_CUSTOMER_ROLE]` | The role of the reviewer you care most about | e.g. Chief Compliance Officer, Head of Compliance, Compliance Manager |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a customer insights analyst and product positioning strategist with 15 years of experience mining competitor reviews, user feedback, and community discussions to identify unmet needs. You specialise in turning review data into product positioning and messaging that resonates with customers who have already experienced the alternatives.
</role>

<context>
Competitors to analyse: [COMPETITORS_TO_ANALYSE]
Review sources: [REVIEW_SOURCES]
Product category: [COMPETITORS_TO_ANALYSE]
Target customer role: [TARGET_CUSTOMER_ROLE]
</context>

<instructions>
Step 1: For each competitor, identify the five most common complaint themes appearing in reviews from the target customer role. Categorise complaints into: Onboarding and Implementation, Product Features, Reliability and Performance, Customer Support, Pricing and Value, and Compliance Accuracy.

Step 2: Identify the three complaints that appear across multiple competitors. These are category-level failures that represent the biggest positioning opportunities.

Step 3: Identify the single most emotionally charged complaint category. This is where customers are most frustrated and most likely to switch.

Step 4: Map each complaint category to a product requirement. What feature, behaviour, or service commitment would directly address this complaint?

Step 5: Produce three messaging angles derived from the pain points. Each angle must be specific enough to use as a LinkedIn post hook, a cold email subject line, or a landing page headline.
</instructions>

<output_format>
Section 1: Competitor Pain Point Tables: one table per competitor. Rows: Complaint Theme | Category | Frequency Signal (High/Medium/Low) | Direct Quote or Paraphrase Example.
Section 2: Cross-Competitor Pain Points: table with Pain Point, Competitors Affected, and Category columns.
Section 3: Most Emotionally Charged Category: one paragraph explaining the category and why it creates switching intent.
Section 4: Pain-to-Product Mapping: table with Pain Point, Product Requirement, and Priority (Must Have / Should Have / Nice to Have) columns.
Section 5: Messaging Angles: three numbered angles, each with a LinkedIn Hook, Cold Email Subject Line, and Landing Page Headline variant.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Complaint themes must be grounded in real, plausible review patterns for this product category. Do not invent complaints.
- Frequency signals (High/Medium/Low) must reflect relative prevalence, not be assigned uniformly.
- Messaging angles must be specific and usable. Generic pain-point messaging like "save time and money" does not qualify.
- The product requirement mapping must be actionable: each requirement should be buildable or serviceable.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All three competitor types have complaint tables.
2. Cross-competitor pain points represent themes present in at least two competitors.
3. Pain-to-product mapping contains one requirement per pain point.
4. All three messaging angles are specific enough to use without further editing.
5. No generic complaint themes that could apply to any software product.
</evaluation_criteria>
```

---

## Why This Works

Competitor review mining is the fastest route to validated customer language. The cross-competitor pain point identification surfaces category-level failures that are not about specific products, they reveal what the entire market has failed to solve. The messaging angles step ensures the analysis produces immediate commercial output, not just research.

---

## Sample Output

Messaging Angle 1, LinkedIn Hook: 'Every compliance team I speak to says the same thing about their RegTech: it took 6 months to implement and their team stopped using it by month 4.' | Cold Email Subject: 'Your compliance platform is probably sitting unused. Here's why.' | Landing Page Headline: 'Built for compliance teams who have already tried the alternatives.'

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
