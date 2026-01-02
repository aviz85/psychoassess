---
argument-hint: "[test-name] [score-pattern or description of findings]"
description: Generate interpretation hypotheses from assessment data. Uses interpretation skill.
allowed-tools: Read, Grep
---

# Score Interpretation Command

Interpret the following assessment data: $ARGUMENTS

## Instructions

Use the interpretation skill to:

1. **Analyze the score pattern** - Identify the key features of this profile
2. **Generate multiple hypotheses** - Never settle on single explanation
3. **Identify evidence** - What supports/contradicts each hypothesis
4. **Connect to function** - What does this mean for daily life/academics
5. **Note limitations** - What we can't conclude from these data
6. **Suggest next steps** - What additional data would help clarify

## Interpretation Principles

- All interpretations are **hypotheses**, not diagnoses
- Consider **multiple explanations** before concluding
- Integrate with **behavioral observations** when available
- Use appropriate **hedging language**
- Connect findings to **referral questions**

## Output Format

Provide interpretation as:
1. Score overview
2. Key findings (with supporting data)
3. Competing hypotheses (ranked by probability)
4. Questions for further exploration
5. Preliminary implications

Remember: AI provides organized information for clinical decision-making; final interpretation rests with the psychologist.
