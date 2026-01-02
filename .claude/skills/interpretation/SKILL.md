---
name: interpretation
description: Generate interpretation hypotheses from test score patterns. Use when analyzing scores, identifying patterns, generating hypotheses, understanding what scores mean, or when the user asks about interpretation, patterns, or score meaning.
allowed-tools: Read, Grep
---

# Score Interpretation Skill

## Purpose
Transform quantitative scores into meaningful clinical hypotheses through systematic analysis.

See [PATTERN_LIBRARY.md](PATTERN_LIBRARY.md) for common score patterns and their interpretations.
See [DECISION_TREES.md](DECISION_TREES.md) for diagnostic pathways.

## Interpretation Framework

### Level 1: Global Ability Level

Start with the big picture:
- What is the overall cognitive functioning level?
- How wide is the confidence interval?
- What does this mean for daily functioning?

**Key Questions**:
- Is FSIQ interpretable (index variability <23 points)?
- If not, use GAI or report indices separately
- What classification applies?

### Level 2: Index-Level Analysis

For each index, document:

```markdown
### [Index Name]: [Score] ([Classification])
- **95% CI**: [range]
- **Percentile**: [X]th percentile
- **Meaning**: [What this measures]
- **Functional implications**: [Real-world impact]
- **Relation to referral question**: [How this addresses concerns]
```

### Level 3: Pattern Analysis

#### Index Comparisons
| Comparison | Difference | Significant? | Base Rate | Interpretation |
|------------|------------|--------------|-----------|----------------|
| VCI vs VSI | | | | |
| VCI vs FRI | | | | |
| VCI vs WMI | | | | |
| VCI vs PSI | | | | |
| GAI vs CPI | | | | |

**Interpretation Guidelines**:
- Statistical significance (p<.05) = rare by chance
- Base rate <15% = clinically noteworthy
- Base rate <5% = highly unusual

#### Within-Index Scatter
For indices with significant subtest scatter (>5 points):
- Which subtest is stronger/weaker?
- What might explain the difference?
- Does this pattern appear elsewhere?

### Level 4: Hypothesis Generation

Generate **multiple competing hypotheses** for observed patterns:

```markdown
## Hypothesis A: [Primary Hypothesis]
**Evidence supporting**:
- [Finding 1]
- [Finding 2]

**Evidence against**:
- [Finding 1]

**Probability estimate**: [High/Medium/Low]

## Hypothesis B: [Alternative Hypothesis]
**Evidence supporting**:
- [Finding 1]

**Evidence against**:
- [Finding 1]

**Probability estimate**: [High/Medium/Low]
```

### Level 5: Integration

#### Cross-Battery Convergence
| Finding | Measure 1 | Measure 2 | Measure 3 | Convergent? |
|---------|-----------|-----------|-----------|-------------|
| | | | | |

#### Behavioral Alignment
- Do test scores match observed behaviors?
- Any unexpected discrepancies?

#### Historical Consistency
- Consistent with developmental history?
- Matches previous testing (if any)?
- Consistent with academic records?

## Common Interpretation Patterns

### High VCI, Low VSI
**Consider**:
- Nonverbal learning disability profile
- Visual-spatial processing disorder
- Right hemisphere concerns

### High VSI, Low VCI
**Consider**:
- Language-based learning disability
- Limited language exposure
- Hearing/auditory processing concerns

### Low WMI
**Consider**:
- ADHD (working memory subtype)
- Anxiety affecting concentration
- Auditory processing weakness

### Low PSI
**Consider**:
- ADHD (processing speed subtype)
- Motor coordination issues
- Perfectionism/anxiety
- Depression/low motivation

### GAI >> CPI
**Consider**:
- Processing weakness despite intact reasoning
- ADHD profile
- Executive function weakness

### Flat Profile with Low FSIQ
**Consider**:
- Intellectual disability
- Global developmental delay
- Limited educational opportunity

## Interpretation Cautions

### Avoid These Errors

1. **Over-interpreting single scores**
   - One low subtest ≠ diagnosis
   - Look for converging evidence

2. **Ignoring base rates**
   - 25% of normal population has 23+ point FSIQ scatter
   - Significance ≠ abnormality

3. **Confirmation bias**
   - Consider alternative explanations
   - Look for disconfirming evidence

4. **Ignoring context**
   - Scores don't exist in vacuum
   - Consider behavioral observations, history

5. **Definitive statements**
   - Use hedging language
   - "Results suggest..." not "Child has..."

## Output Template

```markdown
## Interpretation Summary

### Score Overview
[Brief description of overall profile]

### Key Findings
1. **[Finding 1]**: [Score evidence] → [Interpretation]
2. **[Finding 2]**: [Score evidence] → [Interpretation]
3. **[Finding 3]**: [Score evidence] → [Interpretation]

### Pattern Analysis
[Description of significant patterns with base rates]

### Hypotheses
#### Most Likely: [Hypothesis]
- Supporting evidence: [list]
- Confidence: [High/Medium/Low]

#### Alternative: [Hypothesis]
- Supporting evidence: [list]
- Confidence: [High/Medium/Low]

### Integration with Other Data
[How scores fit with history, observations, other measures]

### Questions Remaining
- [What additional information would help clarify?]

### Implications
- **Educational**: [implications]
- **Clinical**: [implications]
- **Recommendations**: [preliminary ideas]
```

## Important Reminders

- All interpretations are **hypotheses**, not diagnoses
- Clinical judgment **supersedes** algorithmic interpretation
- Consider **multiple explanations** before concluding
- Integrate with **history and observation**
- Use **appropriate hedging** in reports
