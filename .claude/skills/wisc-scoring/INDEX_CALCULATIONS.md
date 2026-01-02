# WISC-V Index Score Calculation Reference

## Sum of Scaled Scores to Composite Score Conversion

### Verbal Comprehension Index (VCI)
| Sum | Score | Sum | Score | Sum | Score |
|-----|-------|-----|-------|-----|-------|
| 2 | 45 | 15 | 84 | 28 | 123 |
| 3 | 48 | 16 | 87 | 29 | 126 |
| 4 | 51 | 17 | 90 | 30 | 129 |
| 5 | 54 | 18 | 93 | 31 | 132 |
| 6 | 57 | 19 | 96 | 32 | 135 |
| 7 | 60 | 20 | 99 | 33 | 138 |
| 8 | 63 | 21 | 102 | 34 | 141 |
| 9 | 66 | 22 | 105 | 35 | 144 |
| 10 | 69 | 23 | 108 | 36 | 147 |
| 11 | 72 | 24 | 111 | 37 | 150 |
| 12 | 75 | 25 | 114 | 38 | 155 |
| 13 | 78 | 26 | 117 | | |
| 14 | 81 | 27 | 120 | | |

*Note: Tables for VSI, FRI, WMI, PSI follow same pattern with adjusted values*

### Full Scale IQ (FSIQ) - 7 Subtests
Sum range: 7-133

| Sum | FSIQ | Sum | FSIQ | Sum | FSIQ |
|-----|------|-----|------|-----|------|
| 7 | 40 | 50 | 79 | 90 | 112 |
| 10 | 45 | 55 | 83 | 95 | 116 |
| 15 | 50 | 60 | 87 | 100 | 120 |
| 20 | 54 | 65 | 91 | 105 | 124 |
| 25 | 58 | 70 | 95 | 110 | 128 |
| 30 | 62 | 75 | 99 | 115 | 132 |
| 35 | 66 | 80 | 103 | 120 | 136 |
| 40 | 71 | 85 | 107 | 125 | 140 |
| 45 | 75 | | | 130+ | 145+ |

## Prorated Scores

When a subtest is spoiled or invalid, use prorated procedures:
1. Calculate available subtest sum
2. Multiply by (total subtests / administered subtests)
3. Round to nearest whole number
4. Look up composite score

**Example**: VCI with only Similarities (12) administered
- Prorated sum = 12 × (2/1) = 24
- VCI = 111

## Standard Error of Measurement (SEM)

| Index | SEM | 90% CI | 95% CI |
|-------|-----|--------|--------|
| FSIQ | 2.60 | ±4 | ±5 |
| VCI | 3.67 | ±6 | ±7 |
| VSI | 4.65 | ±8 | ±9 |
| FRI | 4.24 | ±7 | ±8 |
| WMI | 4.47 | ±7 | ±9 |
| PSI | 5.20 | ±9 | ±10 |
| GAI | 2.92 | ±5 | ±6 |
| CPI | 3.97 | ±7 | ±8 |

## Confidence Interval Formula
CI = Score ± (z × SEM)
- 90% CI: z = 1.645
- 95% CI: z = 1.96

## Percentile Rank Formula
For standard scores (mean=100, SD=15):
%ile ≈ NORMSDIST((Score - 100) / 15) × 100
