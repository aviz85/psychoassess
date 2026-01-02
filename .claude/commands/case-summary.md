---
description: Generate integrated case conceptualization from all available assessment data.
allowed-tools: Read, Grep
---

# Case Summary Command

Generate a comprehensive case conceptualization.

## Instructions

Synthesize all available information into a coherent clinical narrative:

1. **Identify available data** - What information do we have?
2. **State referral questions** - What were we asked to answer?
3. **Integrate findings** - Weave together all data sources
4. **Address each question** - How do findings answer referral concerns?
5. **Note convergent evidence** - Where do multiple sources agree?
6. **Identify divergent data** - Any contradictions to explain?
7. **Formulate impressions** - What is the most likely explanation?
8. **Prioritize recommendations** - What are the most important next steps?

## Case Conceptualization Framework

### 1. Presenting Picture
- Who is this child?
- What brought them to evaluation?
- What is the key concern?

### 2. Developmental Context
- How did we get here?
- What is the trajectory?
- What factors are relevant?

### 3. Assessment Findings
- What did cognitive testing show?
- What did achievement testing reveal?
- What did behavioral measures indicate?
- What did observations suggest?

### 4. Pattern Synthesis
- What is the overall picture?
- How do pieces fit together?
- What explains the presenting concerns?

### 5. Diagnostic Formulation
- What conditions best explain the picture?
- What evidence supports this?
- What was ruled out?

### 6. Recommendations Summary
- What are the top 3-5 most important interventions?
- What is the priority order?
- What follow-up is needed?

## Output Format

```markdown
## Case Conceptualization: [Case ID]

### Referral Questions
1. [Question 1]
2. [Question 2]

### Case Summary
[Integrated narrative - 2-3 paragraphs covering key findings]

### Answers to Referral Questions

**Question 1**: [Question]
[Response with supporting evidence]

**Question 2**: [Question]
[Response with supporting evidence]

### Diagnostic Impressions
- [Primary impression with rationale]
- [Secondary consideration if applicable]

### Priority Recommendations
1. [Most important]
2. [Second priority]
3. [Third priority]

### Follow-Up
- [Timeline and monitoring plan]
```
