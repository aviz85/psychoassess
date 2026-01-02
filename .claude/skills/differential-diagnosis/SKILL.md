---
name: differential-diagnosis
description: Guide differential diagnosis considerations for psychoeducational conditions. Use when considering diagnostic categories, ruling out conditions, distinguishing between similar presentations, or when the user mentions diagnosis, differential, or asks about distinguishing conditions.
allowed-tools: Read, Grep
---

# Differential Diagnosis Skill

## Purpose
Support systematic consideration of diagnostic possibilities while maintaining clinical judgment primacy.

See [CRITERIA_REFERENCE.md](CRITERIA_REFERENCE.md) for DSM-5 criteria summaries.

## Core Principles

1. **AI does not diagnose** - Provides organized information for clinical decision-making
2. **Multiple hypotheses** - Always consider alternatives
3. **Rule-out process** - Systematically eliminate possibilities
4. **Comorbidity awareness** - Conditions frequently co-occur

## Differential Diagnosis Framework

### Step 1: Identify Presenting Concerns
- Academic: Reading, math, writing, overall achievement
- Attention: Focus, concentration, impulsivity
- Behavioral: Conduct, oppositionality, social skills
- Emotional: Anxiety, depression, mood regulation
- Developmental: Language, motor, adaptive skills

### Step 2: Generate Hypothesis List

For each presenting concern, consider:

**Academic Difficulties**
- Specific Learning Disability (Reading/Math/Writing)
- Intellectual Disability
- ADHD (affecting academic output)
- Anxiety (affecting performance)
- Language Disorder
- Limited educational opportunity

**Attention Difficulties**
- ADHD (Inattentive, Hyperactive-Impulsive, Combined)
- Anxiety Disorder
- Depression
- Sleep disorders
- Medical conditions
- Hearing/vision problems
- Trauma response

**Behavioral Difficulties**
- ADHD
- Oppositional Defiant Disorder
- Conduct Disorder
- Autism Spectrum Disorder
- Anxiety (avoidance manifesting as behavior)
- Trauma response

**Emotional Difficulties**
- Generalized Anxiety Disorder
- Social Anxiety Disorder
- Separation Anxiety Disorder
- Major Depressive Disorder
- Adjustment Disorder
- Trauma/PTSD

### Step 3: Evaluate Evidence

For each hypothesis, document:

```markdown
## [Condition Name]

### Supporting Evidence
- [Finding 1]
- [Finding 2]

### Contradicting Evidence
- [Finding 1]
- [Finding 2]

### Information Needed
- [What would confirm/disconfirm]

### Probability: [High/Medium/Low]
```

### Step 4: Rule-Out Analysis

Check exclusionary criteria:
- Medical conditions that could explain symptoms
- Sensory impairments
- Environmental factors
- Better accounted for by another condition

### Step 5: Consider Comorbidity

Common co-occurring conditions:
- ADHD + SLD (30-50% comorbidity)
- ADHD + Anxiety (25-50% comorbidity)
- ADHD + ODD (40-60% comorbidity)
- Anxiety + Depression (frequent comorbidity)
- ASD + ADHD (common)
- SLD + Anxiety (secondary to frustration)

## Key Differentials

### ADHD vs. Anxiety

| Feature | ADHD | Anxiety |
|---------|------|---------|
| Onset | Early childhood | Any age |
| Trigger | Pervasive | Situational |
| Internal experience | Mind wanders | Mind races with worry |
| Restlessness | Purposeless activity | Nervous energy |
| Inattention cause | Distracted by stimuli | Distracted by thoughts |
| Sleep | May have difficulty | Often difficulty |
| Novelty | Improves focus | Worsens anxiety |
| Processing speed | Often low | Variable (may be slow due to checking) |
| Motivation | Can focus on preferred tasks | Fear-driven avoidance |

### ADHD vs. Learning Disability

| Feature | ADHD | LD |
|---------|------|-----|
| Academic pattern | Inconsistent across subjects | Specific subject weakness |
| Attention | Universally poor | Poor when demands high |
| Effort | Variable | Often high |
| Organization | Broadly impaired | May be intact |
| Homework | Knows it, doesn't show it | Skill gaps evident |
| Intervention response | Structure, behavior support | Direct skill instruction |

### Anxiety vs. Depression

| Feature | Anxiety | Depression |
|---------|---------|------------|
| Core emotion | Fear/worry | Sadness/emptiness |
| Energy | Often elevated (nervous) | Low (fatigued) |
| Focus | Future threats | Past failures |
| Motivation | High (avoidance-driven) | Low (anhedonia) |
| Sleep | Difficulty falling asleep | Early waking, hypersomnia |
| Appetite | May be reduced | Variable |
| Social | May avoid due to fear | Withdrawal due to apathy |

### Autism vs. Social Anxiety

| Feature | ASD | Social Anxiety |
|---------|-----|----------------|
| Onset | Early developmental | Often later |
| Desire for friends | Variable | Often wants friends |
| Perspective-taking | Impaired | Intact but feared |
| Repetitive behaviors | Present | Usually absent |
| Sensory issues | Common | Usually absent |
| Special interests | Intense, unusual | Normal interests |
| Improvement with familiarity | Moderate | Significant |

### ID vs. Specific Learning Disability

| Feature | ID | SLD |
|---------|-----|-----|
| Cognitive profile | Flat, uniformly low | Variable with specific weakness |
| Adaptive behavior | Impaired | Relative strength |
| Learning potential | Limited | Average or higher reasoning |
| Academic ceiling | Significantly limited | Grade-level possible with support |
| Independence | Limited | Expected in most areas |

### Depression vs. ADHD

| Feature | Depression | ADHD |
|---------|------------|------|
| Onset | Can be any age | Childhood |
| Course | Episodic | Chronic |
| Energy | Low | Variable/high |
| Motivation | Globally reduced | Intact for preferred activities |
| Mood | Persistently low | Variable |
| Sleep | Disturbed | May be disturbed |
| Self-esteem | Negative thoughts | May be preserved |

## Diagnostic Hierarchy Considerations

When multiple conditions could apply:

1. **Is there a medical condition that explains symptoms?**
   - Always rule out first
   - Thyroid, sleep disorders, medication effects, hearing/vision

2. **Is there a pervasive developmental condition?**
   - ASD is a foundational consideration
   - Other symptoms may be secondary

3. **Is there an intellectual disability?**
   - Defines expected functioning level
   - Other diagnoses may still apply

4. **Are learning differences present?**
   - May explain academic struggles
   - ADHD and LD frequently co-occur

5. **Are attention/executive function issues present?**
   - ADHD can affect many areas
   - Consider comorbid conditions

6. **Are emotional factors primary or secondary?**
   - Anxiety/depression can result from other conditions
   - Can also exist independently

## Output Format

```markdown
## Differential Diagnosis Summary

### Primary Presenting Concerns
1. [Concern]
2. [Concern]

### Diagnostic Considerations

#### Most Likely: [Diagnosis]
- **Evidence for**: [list]
- **Evidence against**: [list]
- **Confidence**: [High/Medium/Low]

#### Alternative 1: [Diagnosis]
- **Evidence for**: [list]
- **Evidence against**: [list]
- **Confidence**: [High/Medium/Low]

#### Alternative 2: [Diagnosis]
- **Evidence for**: [list]
- **Evidence against**: [list]
- **Confidence**: [High/Medium/Low]

### Ruled Out
- [Condition]: [Reason]

### Comorbidity Considerations
- [Condition] may co-occur because [reason]

### Additional Evaluation Recommended
- [What would clarify diagnosis]

### Diagnostic Impression
[Clinical summary with appropriate hedging]
```

## Important Reminders

- Diagnosis requires licensed professional judgment
- AI provides organized information, not diagnoses
- Consider cultural and contextual factors
- Document reasoning for all conclusions
- When uncertain, recommend further evaluation
