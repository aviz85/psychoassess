---
name: wisc-scoring
description: Calculate WISC-V composite scores, confidence intervals, percentiles, and discrepancy analyses. Use when entering WISC scores, calculating indices, checking score calculations, or when the user mentions WISC, IQ scores, or cognitive testing scores.
allowed-tools: Read, Bash(python:*)
---

# WISC-V Scoring Skill

## Purpose
Accurate calculation and verification of WISC-V scores with clinical interpretation support.

See [INDEX_CALCULATIONS.md](INDEX_CALCULATIONS.md) for detailed formulas.
See [SUBTEST_REFERENCE.md](SUBTEST_REFERENCE.md) for subtest descriptions.

## Score Entry Format

Provide scaled scores (1-19 range, mean=10, SD=3) for administered subtests:

### Primary Subtests (required for FSIQ)
```
Similarities (SI):
Vocabulary (VC):
Block Design (BD):
Visual Puzzles (VP):
Matrix Reasoning (MR):
Figure Weights (FW):
Digit Span (DS):
Picture Span (PS):
Coding (CD):
Symbol Search (SS):
```

### Secondary Subtests (optional)
```
Information (IN):
Comprehension (CO):
Picture Concepts (PC):
Letter-Number Sequencing (LN):
Cancellation (CA):
```

## Primary Index Score Calculations

| Index | Subtests | Sum Range |
|-------|----------|-----------|
| **VCI** (Verbal Comprehension) | SI + VC | 2-38 |
| **VSI** (Visual Spatial) | BD + VP | 2-38 |
| **FRI** (Fluid Reasoning) | MR + FW | 2-38 |
| **WMI** (Working Memory) | DS + PS | 2-38 |
| **PSI** (Processing Speed) | CD + SS | 2-38 |
| **FSIQ** (Full Scale IQ) | SI+VC+BD+MR+FW+DS+CD | 7-133 |

## Ancillary Index Scores

| Index | Subtests | When to Use |
|-------|----------|-------------|
| **QRI** | FW + AR | Quantitative reasoning questions |
| **AWMI** | DS + LN | Auditory vs visual working memory |
| **NVI** | BD+VP+MR+FW+PS+CD | Language-reduced estimate |
| **GAI** | SI+VC+BD+VP+MR+FW | Ability without WM/PS |
| **CPI** | DS+PS+CD+SS | Processing efficiency |

## Score Interpretation Tables

### Standard Score to Percentile
| SS | %ile | SS | %ile | SS | %ile |
|----|------|----|----- |----| -----|
| 145 | 99.9 | 115 | 84 | 85 | 16 |
| 140 | 99.6 | 110 | 75 | 80 | 9 |
| 135 | 99 | 105 | 63 | 75 | 5 |
| 130 | 98 | 100 | 50 | 70 | 2 |
| 125 | 95 | 95 | 37 | 65 | 1 |
| 120 | 91 | 90 | 25 | 60 | 0.4 |

### Classification System
| Range | Classification | Description |
|-------|---------------|-------------|
| 130+ | Extremely High | Upper 2% |
| 120-129 | Very High | Well above average |
| 110-119 | High Average | Above average |
| 90-109 | Average | Typical range |
| 80-89 | Low Average | Below average |
| 70-79 | Borderline | Significantly below |
| ≤69 | Extremely Low | Lower 2% |

### 95% Confidence Intervals
| Index | SEM | 95% CI = Score ± |
|-------|-----|------------------|
| FSIQ | 2.60 | ±5 |
| VCI | 3.67 | ±7 |
| VSI | 4.65 | ±9 |
| FRI | 4.24 | ±8 |
| WMI | 4.47 | ±9 |
| PSI | 5.20 | ±10 |

## Discrepancy Analysis

### Index-Level Discrepancies
Critical values for significance (p<.05):
| Comparison | Critical Difference |
|------------|-------------------|
| VCI vs VSI | 11 points |
| VCI vs FRI | 11 points |
| VCI vs WMI | 12 points |
| VCI vs PSI | 13 points |
| VSI vs FRI | 13 points |
| VSI vs WMI | 14 points |
| VSI vs PSI | 15 points |
| FRI vs WMI | 13 points |
| FRI vs PSI | 14 points |
| WMI vs PSI | 15 points |

### Interpreting Discrepancies
1. **Statistical significance** - Is the difference rare by chance?
2. **Base rate** - How common is this difference in the population?
3. **Clinical significance** - Does it matter functionally?

Rule of thumb: Base rates <15% warrant clinical attention.

## Output Format

```markdown
## WISC-V Score Summary

### Client: [Case ID] | Date: [Date] | Age: [Age]

### Primary Index Scores
| Index | Score | 95% CI | Percentile | Classification |
|-------|-------|--------|------------|----------------|
| VCI | | | | |
| VSI | | | | |
| FRI | | | | |
| WMI | | | | |
| PSI | | | | |
| **FSIQ** | | | | |

### Subtest Profile
| Subtest | Scaled Score | Percentile | Strength/Weakness |
|---------|--------------|------------|-------------------|
| | | | |

### Significant Discrepancies
| Comparison | Difference | Significant? | Base Rate |
|------------|------------|--------------|-----------|
| | | | |

### Profile Analysis
- **Strengths**:
- **Weaknesses**:
- **Pattern notes**:
```

## Example Calculation

**Input**: SI:12 VC:11 BD:8 VP:7 MR:10 FW:9 DS:7 PS:6 CD:8 SS:7

**Calculations**:
- VCI = SI(12) + VC(11) = 23 → Standard Score: 106
- VSI = BD(8) + VP(7) = 15 → Standard Score: 81
- FRI = MR(10) + FW(9) = 19 → Standard Score: 96
- WMI = DS(7) + PS(6) = 13 → Standard Score: 78
- PSI = CD(8) + SS(7) = 15 → Standard Score: 83
- FSIQ = 12+11+8+10+9+7+8 = 65 → Standard Score: 88

**Significant Discrepancies**:
- VCI (106) - VSI (81) = 25 points ✓ (>11, significant)
- VCI (106) - WMI (78) = 28 points ✓ (>12, significant)
- VCI (106) - PSI (83) = 23 points ✓ (>13, significant)

**Interpretation**: Significant verbal > nonverbal pattern with processing weaknesses.
