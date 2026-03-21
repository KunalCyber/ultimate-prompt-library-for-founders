# Contributing to the The Ultimate Prompt Library

First: thank you. This library gets better with every prompt added, improved, or refined.

## Quality Bar

Every prompt in this library must meet the same standard as the existing 50. The bar is not "good enough": it is "a founder or executive could hand this to their team and get a structured, specific, immediately usable output every single time."

## How to Add a New Prompt

1. **Fork the repository** and create a branch: `git checkout -b prompt/your-prompt-name`

2. **Use the template**: Copy `.github/PROMPT_TEMPLATE.md` into the appropriate domain folder. Name the file `[NUMBER]-[prompt-slug].md`.

3. **Meet all 8 engineering requirements:**
   - [ ] Specific expert role (not "business consultant" but "SaaS pricing strategist with 15 years B2B experience")
   - [ ] Full XML tag structure: `<role>`, `<context>`, `<instructions>`, `<output_format>`, `<constraints>`, `<evaluation_criteria>`
   - [ ] At least 4 `[BRACKETED_VARIABLES]` with descriptions and examples
   - [ ] Exact output format: tables, columns, scoring scales, section headers
   - [ ] Numbered instruction steps (minimum 4)
   - [ ] Evaluation criteria with at least 5 numbered checks
   - [ ] Chain-of-thought instruction for Advanced-level prompts
   - [ ] British English throughout. No em dashes. No filler phrases.

4. **Test your prompt**: Run it with Claude or GPT-4o with real inputs. The output must be structured, specific, and immediately usable without editing.

5. **Submit a pull request** with:
   - Prompt title and domain
   - Skill level (Essential / Practitioner / Advanced)
   - A real sample output (not placeholder text)

## How to Improve an Existing Prompt

Found a phrase that is vague, a scoring criterion that is ambiguous, or an output format that could be sharper? Open a PR with the specific change and the reason for it.

## What We Do Not Accept

- Generic prompts that produce generic output
- Prompts without the full XML structure
- Prompts with American English spellings
- Prompts that use em dashes or banned filler phrases
- Prompts with placeholder sample outputs

## Banned Phrases

These phrases must not appear anywhere in any prompt in this library:

- "It is worth noting that..."
- "In today's rapidly evolving landscape..."
- "Leverage" used as a verb
- "In conclusion..."
- "As we can see..."
- Any variation of "it is important to remember"

## Questions

Open an issue. We will respond.
