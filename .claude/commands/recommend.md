---
argument-hint: "[area-of-need or diagnostic-profile]"
description: Generate evidence-based intervention recommendations. Uses recommendation-generator agent.
allowed-tools: Read, Grep
---

# Recommendation Generator Command

Generate recommendations for: $ARGUMENTS

## Instructions

Generate tailored, evidence-based recommendations that:

1. **Connect to findings** - Each recommendation linked to assessment data
2. **Are specific** - Include implementation details
3. **Are prioritized** - Order by impact and feasibility
4. **Cover multiple domains** - Accommodations, interventions, supports
5. **Include responsibility** - Who implements, where, when

## Recommendation Categories

### Educational Accommodations
- Classroom accommodations
- Testing accommodations
- Environmental modifications
- Assistive technology

### Academic Interventions
- Subject-specific interventions
- Evidence-based programs
- Instructional strategies
- Tutoring approaches

### Executive Function Supports
- Organization systems
- Time management
- Self-monitoring strategies
- Working memory supports

### Social-Emotional Interventions
- Counseling recommendations
- Social skills support
- Anxiety management
- Behavioral strategies

### Home Supports
- Parent strategies
- Homework modifications
- Communication with school
- Community resources

## Output Format

For each recommendation, provide:
- **What**: Specific strategy or accommodation
- **Why**: Brief rationale linked to findings
- **How**: Implementation details
- **Who**: Responsible party
- **Priority**: High/Medium/Low

Organize by:
1. Immediate/high priority needs
2. Short-term interventions
3. Long-term considerations
4. Follow-up/monitoring
