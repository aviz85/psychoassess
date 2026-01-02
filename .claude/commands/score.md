---
argument-hint: "[test-name] [subtest:score pairs or index scores]"
description: Calculate composite scores, confidence intervals, and percentiles for cognitive tests. Uses wisc-scoring skill.
allowed-tools: Read, Bash(python:*)
---

# Score Calculation Command

Calculate scores for: $ARGUMENTS

## Instructions

Use the wisc-scoring skill to:

1. **Parse the input** - Identify the test name and score values provided
2. **Calculate composites** - Compute all applicable index/composite scores
3. **Generate confidence intervals** - Provide 95% CIs for all composites
4. **Compute percentiles** - Convert scores to percentile ranks
5. **Identify discrepancies** - Flag statistically significant differences
6. **Note patterns** - Identify strengths/weaknesses

## Expected Input Formats

**WISC-V Subtest Scores** (scaled scores 1-19):
```
/score wisc-v SI:12 VC:11 BD:8 VP:7 MR:10 FW:9 DS:7 PS:6 CD:8 SS:7
```

**WISC-V Index Scores** (for discrepancy analysis):
```
/score wisc-v VCI:106 VSI:81 FRI:96 WMI:78 PSI:83
```

## Output Format

Present results as a clear table with:
- Index/Composite name
- Standard score
- 95% Confidence interval
- Percentile rank
- Classification
- Any significant discrepancies noted
