---
argument-hint: "[condition-comparison: e.g., adhd-vs-anxiety, ld-vs-id]"
description: Guide differential diagnosis considerations. Uses differential-diagnosis skill.
allowed-tools: Read, Grep
---

# Differential Diagnosis Command

Analyze differential diagnosis for: $ARGUMENTS

## Instructions

Use the differential-diagnosis skill to:

1. **Define the conditions** - What are we comparing?
2. **List key differentiating features** - What distinguishes them?
3. **Apply to current case** - What evidence do we have?
4. **Generate probability estimates** - Which is more likely?
5. **Consider comorbidity** - Could both be present?
6. **Identify clarifying data** - What would help distinguish?

## Common Differentials

### adhd-vs-anxiety
Key features: onset, trigger patterns, internal experience, novelty response

### adhd-vs-ld
Key features: academic pattern, attention universality, intervention response

### anxiety-vs-depression
Key features: core emotion, energy, temporal focus, motivation

### autism-vs-social-anxiety
Key features: social desire, onset, repetitive behaviors, sensory issues

### id-vs-ld
Key features: profile flatness, adaptive behavior, academic ceiling

### depression-vs-adhd
Key features: onset, course, energy, motivation pattern

## Output Format

```markdown
## Differential Analysis: [Condition A] vs [Condition B]

### Key Distinguishing Features
| Feature | [Condition A] | [Condition B] | This Case |
|---------|---------------|---------------|-----------|
| | | | |

### Evidence Analysis

**Supporting [Condition A]**:
- [Evidence 1]
- [Evidence 2]

**Supporting [Condition B]**:
- [Evidence 1]
- [Evidence 2]

### Comorbidity Consideration
[Can both be present? How common?]

### Most Likely Impression
[Primary conclusion with confidence level]

### Clarifying Information Needed
- [What would help distinguish?]
```

## Important Reminder

This analysis provides organized information for clinical decision-making. Diagnosis requires:
- Licensed professional judgment
- Integration of multiple data sources
- Clinical interview
- Consideration of context
