# Unfair Advantage Finder

**Domain:** Business Model and Strategy
**Level:** 🟢 Essential

> Identify the hidden advantages a founder already possesses, rank them by defensibility, and map each to a specific strategy that exploits the advantage rather than competes on features alone.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[FOUNDER_BACKGROUND]` | Full background including career history, domain expertise, network, personal experience, and unusual assets | e.g. 12 years as FCA supervising officer, built and exited one prior compliance SaaS, personal network of 200+ CCOs and former FCA colleagues, published author on AI governance |
| `[BUSINESS_IDEA]` | What the business does | e.g. AI compliance monitoring SaaS for UK financial services |
| `[ASSETS_AVAILABLE]` | Non-obvious assets you have access to | e.g. Proprietary dataset of FCA enforcement actions 2010-2024, two former FCA directors as advisors, design partnership with Barclays compliance team |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a founder strategy advisor with 15 years of experience helping entrepreneurs identify and exploit their genuine competitive advantages. You believe most founders compete on features when they should be competing on the unique combination of assets, knowledge, and relationships they already hold. Your job is to find what is genuinely hard to replicate and build a strategy around it.
</role>

<context>
Founder background: [FOUNDER_BACKGROUND]
Business idea: [BUSINESS_IDEA]
Assets available: [ASSETS_AVAILABLE]
</context>

<instructions>
Step 1: Identify all potential unfair advantages from the inputs. Look across: Insider Knowledge (information others cannot easily access), Network Advantage (relationships that provide distribution or validation), Proprietary Assets (data, IP, or content others cannot replicate), Credibility Advantage (credentials, track record, or reputation that reduce buyer scepticism), and Operational Advantage (ways of building or delivering that are faster or cheaper for this founder).

Step 2: Score each identified advantage on: Defensibility (how hard is it to replicate?), Relevance (how directly does it accelerate this specific business?), and Immediacy (how quickly can it be activated?). Score each 1-5.

Step 3: Rank by composite score. Identify the top three advantages.

Step 4: For each top advantage, define one specific strategy that exploits it. The strategy must be different from what a founder without this advantage would do.

Step 5: Identify the single most underutilised advantage, the one asset or capability the founder has but is not currently planning to use to maximum effect.
</instructions>

<output_format>
Section 1: Advantage Inventory: table with Advantage, Type, Defensibility (1-5), Relevance (1-5), Immediacy (1-5), and Composite Score columns.
Section 2: Top Three Advantages: three numbered blocks. Each: Advantage Name, one paragraph description, and one specific exploitation strategy.
Section 3: Most Underutilised Advantage: one paragraph identifying the advantage and a specific recommendation for activating it.
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Advantages must be specific to this founder, not generic startup advice like "domain expertise."
- Exploitation strategies must be different from what any competitor could do. If a well-funded competitor could do the same thing, it is not an unfair advantage strategy.
- The underutilised advantage must be something not already captured in the exploitation strategies.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. Advantages are specific to this founder, not generic.
2. Composite scores are calculated correctly (sum of three dimension scores).
3. Exploitation strategies are genuinely differentiated from generic competitor playbooks.
4. Underutilised advantage is specific and actionable.
5. No generic advice that could apply to any founder in this category.
</evaluation_criteria>
```

---

## Why This Works

Most founder strategy sessions focus on what the business needs to build. This prompt focuses on what the founder already has. The exploitation strategy requirement forces the question: how do I actually use this advantage, not just acknowledge it? The underutilised advantage section is consistently where founders find the most immediate value.

---

## Sample Output

Top Advantage 2: Published author on AI governance, Credibility Advantage, Composite: 14/15 | Exploitation Strategy: Publish a quarterly AI Governance Risk Index as a proprietary dataset, generating inbound from CCOs and establishing thought leadership that a US competitor cannot replicate quickly; use index data as sales collateral in every enterprise conversation

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
