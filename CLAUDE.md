# PsychoAssess - Psychoeducational Assessment Workspace

## Overview
AI-powered workspace supporting psychologists throughout the psychoeducational assessment process. This system provides structured guidance, scoring assistance, interpretation support, and report writing tools.

**Important**: All AI outputs are clinical hypotheses requiring professional judgment. AI supplements but never replaces clinical expertise.

## Assessment Workflow Stages

1. **Intake** → `/intake` - Referral review, background gathering
2. **Observation** → `/observe` - Behavioral observation during testing
3. **Administration** - Test administration (clinician-performed)
4. **Scoring** → `/score` - Score calculation and verification
5. **Interpretation** → `/interpret` - Pattern analysis and hypothesis generation
6. **Diagnosis** → `/differential` - Differential diagnosis consideration
7. **Recommendations** → `/recommend` - Evidence-based intervention planning
8. **Report Writing** → `/draft-section` - Documentation and communication

## Quick Commands

| Command | Purpose | Example |
|---------|---------|---------|
| `/score [test] [scores]` | Calculate composites | `/score wisc-v SI:12 VC:11 BD:8` |
| `/interpret [data]` | Generate hypotheses | `/interpret wisc-v VCI:106 VSI:81 WMI:78` |
| `/observe` | Start observation form | `/observe` |
| `/recommend [area]` | Get recommendations | `/recommend working-memory` |
| `/draft-section [name]` | Draft report section | `/draft-section background` |
| `/case-summary` | Full case conceptualization | `/case-summary` |
| `/differential [concern]` | Diagnostic considerations | `/differential adhd-vs-anxiety` |

## Key Resources

- **Decision Trees**: @knowledge/decision-trees/ - Diagnostic pathways
- **WISC-V Reference**: @knowledge/cognitive/wisc-v/ - Administration and interpretation
- **Behavioral Scales**: @knowledge/behavioral/rating-scales/ - BASC, Conners, etc.
- **Emotional Assessment**: @knowledge/emotional/ - Self-report and projective measures

## Classification Terminology

Use Wechsler standard classifications:
| Score Range | Classification |
|-------------|----------------|
| 130+ | Extremely High |
| 120-129 | Very High |
| 110-119 | High Average |
| 90-109 | Average |
| 80-89 | Low Average |
| 70-79 | Borderline |
| ≤69 | Extremely Low |

## Ethical Reminders

- All interpretations are **hypotheses** requiring clinical judgment
- AI suggestions **supplement**, never replace, professional expertise
- Maintain **client confidentiality** - use case numbers, not names
- Document AI assistance in reports when appropriate
- Final clinical decisions rest with the licensed psychologist

## Confidentiality Protocol

- Store all case data in `cases/` folder (gitignored)
- Use anonymized identifiers (Case001, Case002)
- Never include identifying information in prompts
- Secure all assessment data appropriately

## Report Language Standards

- Use appropriate hedging: "results suggest," "pattern consistent with"
- Maintain parent-friendly language with technical accuracy
- Frame findings with strengths first
- Provide specific, actionable recommendations
