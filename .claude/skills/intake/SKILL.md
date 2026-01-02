---
name: intake
description: Gather and organize referral information, developmental history, and background data. Use when starting a new case, reviewing referral questions, organizing intake information, or when the user mentions intake, referral, or background history.
allowed-tools: Read, Write, Grep
---

# Intake Assessment Skill

## Purpose
Systematically gather and organize pre-assessment information to inform test selection and interpretation.

## Intake Process

### 1. Referral Review
Clarify and document:
- **Primary referral question(s)** - What specifically needs answering?
- **Referral source** - School, parent, physician, therapist?
- **Referral context** - What prompted the referral now?
- **Previous evaluations** - Any prior testing or diagnoses?
- **Current services** - IEP, 504, therapy, medications?

### 2. Developmental History Checklist

#### Prenatal/Birth
- Pregnancy complications?
- Gestational age at birth?
- Birth complications?
- NICU stay?

#### Early Development
- Motor milestones (sitting, walking)
- Language milestones (first words, sentences)
- Any regression noted?

#### Medical History
- Chronic conditions?
- Hospitalizations/surgeries?
- Hearing/vision status?
- Current medications?
- Sleep patterns?

#### Educational History
- Preschool experience?
- Grade retentions?
- Previous special education?
- Academic strengths/weaknesses?

#### Social-Emotional
- Peer relationships?
- Behavioral concerns?
- Anxiety/mood symptoms?
- Trauma history?

#### Family History
- Learning disabilities in family?
- Mental health conditions?
- Developmental disorders?

### 3. Record Review Checklist
Organize information from:
- [ ] School records / report cards
- [ ] Previous psychological evaluations
- [ ] Medical records
- [ ] IEP/504 documents
- [ ] Teacher reports
- [ ] Therapy notes (if available)

## Output: Intake Summary Template

```markdown
## Case: [Case ID]
## Date: [Date]
## Examiner: [Name]

### Referral Information
- **Source**:
- **Primary Question(s)**:
  1.
  2.
- **Previous Diagnoses**:
- **Current Services**:

### Background Summary
- **Developmental**:
- **Medical**:
- **Educational**:
- **Social-Emotional**:
- **Family**:

### Key Factors for Assessment
1.
2.
3.

### Initial Hypotheses
-
-

### Recommended Test Battery
| Domain | Measure | Rationale |
|--------|---------|-----------|
| Cognitive | | |
| Achievement | | |
| Behavioral | | |
| Emotional | | |

### Questions to Explore During Assessment
1.
2.
```

## Example Intake

**Referral**: 8-year-old male, referred by school for suspected learning disability. Struggling with reading despite average classroom performance in math. Previous vision/hearing screening normal.

**Key History**: Full-term birth, normal milestones. Started reading intervention in 1st grade. Father reports similar reading difficulties as a child.

**Initial Hypotheses**:
1. Specific Learning Disability in Reading (dyslexia)
2. Language-based learning weakness
3. Attention factors affecting reading fluency

**Recommended Battery**:
- WISC-V (cognitive profile)
- WIAT-4 (achievement levels)
- CTOPP-2 (phonological processing)
- BASC-3 (rule out behavioral factors)
