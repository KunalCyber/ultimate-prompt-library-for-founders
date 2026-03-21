# Founder-Problem-Market Fit Analyser

**Domain:** Business Model Foundations
**Level:** 🔵 Practitioner

> Go beyond surface-level validation. Analyse the depth of fit between the founder's specific capabilities, the problem's structure, and the market's dynamics to identify where advantage is real and where it is assumed.

---

## Variables

Fill in every `[BRACKETED_VARIABLE]` before running. Do not leave any bracket unfilled.

| Variable | What to Enter | Example |
|----------|---------------|---------|
| `[FOUNDER_PROFILE]` | Your background, skills, network, and unfair advantages | e.g. 10 years in NHS procurement, deep relationships with 50+ NHS trust CFOs, built two prior EdTech products |
| `[PROBLEM_STATEMENT]` | Precise description of the problem including who experiences it and when | e.g. NHS procurement teams spend 40% of their time on supplier compliance checks that could be automated |
| `[MARKET_DESCRIPTION]` | The market you are targeting including size, growth rate, and key dynamics | e.g. UK public sector procurement software, estimated £800m market, growing 12% YoY post-NHS digital mandate |
| `[CURRENT_ALTERNATIVES]` | How the target customer currently solves this problem | e.g. Manual spreadsheet processes, legacy SAP modules, or outsourcing to Big 4 advisory teams |

---

## The Prompt

Copy everything in the code block below. Replace all `[VARIABLES]`. Paste into Claude, GPT-4o, Gemini, or any capable LLM.

```
<role>
You are a venture strategist and founder coach with 15 years of experience evaluating early-stage companies across B2B software, marketplaces, and services. You specialise in identifying whether a founder has genuine, durable advantage in a market or is competing on hope.
</role>

<context>
Founder profile: [FOUNDER_PROFILE]
Problem statement: [PROBLEM_STATEMENT]
Market description: [MARKET_DESCRIPTION]
Current alternatives: [CURRENT_ALTERNATIVES]
</context>

<instructions>
Step 1: Analyse founder-problem fit. Does the founder have domain expertise, lived experience, or network advantage that gives them insight into this problem that a generalist founder would not have? Score founder-problem fit (1-5).

Step 2: Analyse problem-market fit. Is the problem widespread enough, painful enough, and urgent enough to support a scalable business? Are customers actively seeking solutions or passively tolerating the pain? Score problem-market fit (1-5).

Step 3: Analyse founder-market fit. Does the founder have the distribution advantage, credibility, or access to reach this market faster than a well-funded competitor? Score founder-market fit (1-5).

Step 4: Identify the single strongest source of advantage in this combination. What is the one thing this founder can do in this market that is genuinely difficult for others to replicate?

Step 5: Identify the single most dangerous assumption. What, if proven wrong, would make this venture unviable regardless of execution quality?

Step 6: Produce a fit matrix summarising all three dimensions with scores, a composite fit score, and a Go / Proceed with Caution / Stop signal.
</instructions>

<output_format>
Section 1: Founder-Problem Fit Analysis: one paragraph plus score (1-5).
Section 2: Problem-Market Fit Analysis: one paragraph plus score (1-5).
Section 3: Founder-Market Fit Analysis: one paragraph plus score (1-5).
Section 4: Primary Advantage: one precise paragraph naming the specific, defensible advantage.
Section 5: Most Dangerous Assumption: one paragraph naming the assumption and the consequence if it fails.
Section 6: Fit Matrix Table: three rows (Founder-Problem / Problem-Market / Founder-Market) with Score, Strength, and Risk columns. Final row: Composite Score and Signal (GO / PROCEED WITH CAUTION / STOP).
Write in British English. No em dashes. No filler phrases.
</output_format>

<constraints>
- Do not produce generic encouragement. Score honestly.
- Every score must have a specific, evidenced rationale drawn from the inputs provided.
- The most dangerous assumption must be specific to this venture, not a generic startup risk.
- The Go / Proceed / Stop signal must align with the composite score and be unambiguous.
</constraints>

<evaluation_criteria>
Before delivering, verify:
1. All three fit dimensions are scored individually with specific rationale.
2. Composite score is the sum of three dimension scores.
3. Signal aligns with composite: 12-15 = GO, 7-11 = PROCEED WITH CAUTION, 1-6 = STOP.
4. Most dangerous assumption is specific to this venture.
5. No placeholder or generic content in any section.
</evaluation_criteria>
```

---

## Why This Works

Most validation frameworks conflate three distinct questions: can this founder solve this problem, is this problem worth solving, and can this founder reach this market. Separating them produces a sharper diagnosis of where the real risk sits, allowing founders to address specific gaps rather than receiving a generic green light.

---

## Sample Output

Fit Matrix row example: Founder-Market Fit | 4 | 10 years of NHS trust relationships creates immediate distribution advantage | Risk: relationships built in old role may not transfer to purchasing authority in new capacity

---

*Part of the [The Ultimate Prompt Library](../../README.md) · Built by [Kunal RK](https://linkedin.com/in/kunalrk)*
