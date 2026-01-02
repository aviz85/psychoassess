<p align="center">
  <img src="assets/banner.jpg" alt="PsychoAssess Banner" width="100%">
</p>

<h1 align="center">PsychoAssess</h1>

<p align="center">
  <strong>AI-Powered Psychoeducational Assessment Workspace</strong>
</p>

<p align="center">
  <a href="https://aviz85.github.io/psychoassess/">Website (Hebrew)</a> •
  <a href="https://aviz85.github.io/psychoassess/instructions.html">Installation Guide</a> •
  <a href="https://github.com/aviz85/psychoassess/issues">Report Issues</a>
</p>

---

A Claude Code-based knowledge system designed to support psychologists throughout the psychoeducational assessment process. Built using skills, agents, and structured knowledge for real-time clinical support.

## Overview

PsychoAssess provides an interactive, modular workspace for:
- **Scoring assistance** - Calculate composites, confidence intervals, and discrepancies
- **Interpretation support** - Generate hypotheses from score patterns
- **Behavioral observation** - Structured documentation during testing
- **Differential diagnosis** - Systematic consideration of diagnostic possibilities
- **Report writing** - Professional documentation with templates and phrase banks
- **Recommendation generation** - Evidence-based intervention planning

> **Important**: All AI outputs are clinical hypotheses requiring professional judgment. AI supplements but never replaces clinical expertise.

## Quick Start

### Prerequisites
- [Claude Code CLI](https://claude.ai/claude-code) installed
- Git installed

### Installation

```bash
# Clone the repository
git clone https://github.com/aviz85/psychoassess.git

# Navigate to the workspace
cd psychoassess

# Start Claude Code
claude
```

### Available Commands

| Command | Description | Example |
|---------|-------------|---------|
| `/score` | Calculate test scores | `/score wisc-v SI:12 VC:11 BD:8 VP:7` |
| `/interpret` | Generate interpretation hypotheses | `/interpret wisc-v VCI:106 VSI:81` |
| `/observe` | Start behavioral observation form | `/observe` |
| `/recommend` | Generate recommendations | `/recommend working-memory` |
| `/draft-section` | Draft report section | `/draft-section background` |
| `/case-summary` | Generate case conceptualization | `/case-summary` |
| `/differential` | Differential diagnosis guide | `/differential adhd-vs-anxiety` |

## Project Structure

```
psychoassess/
├── CLAUDE.md                    # Main workspace memory
├── .claude/
│   ├── rules/                   # Domain-specific guidelines
│   │   ├── ethical-guidelines.md
│   │   ├── report-standards.md
│   │   ├── cognitive/
│   │   ├── emotional/
│   │   └── behavioral/
│   ├── skills/                  # Reusable assessment capabilities
│   │   ├── intake/
│   │   ├── behavioral-observation/
│   │   ├── wisc-scoring/
│   │   ├── interpretation/
│   │   ├── differential-diagnosis/
│   │   └── report-writing/
│   ├── commands/                # Slash commands
│   └── agents/                  # Specialized sub-agents
│       ├── pattern-analyzer/
│       └── recommendation-generator/
├── knowledge/                   # Professional content library
│   ├── cognitive/
│   ├── emotional/
│   ├── behavioral/
│   └── decision-trees/
└── cases/                       # Case data (gitignored)
```

## Features

### Skills

**Intake** - Systematic gathering of referral information, developmental history, and background data.

**Behavioral Observation** - Structured documentation of test session behaviors with validity considerations.

**WISC Scoring** - Calculation of WISC-V composites, confidence intervals, percentiles, and discrepancy analyses.

**Interpretation** - Multi-hypothesis generation from score patterns with evidence-based reasoning.

**Differential Diagnosis** - Systematic comparison of diagnostic possibilities with decision support.

**Report Writing** - Professional documentation with templates, phrase banks, and style guidance.

### Agents

**Pattern Analyzer** - Cross-battery analysis for complex score profiles, identifying convergent evidence and profile classifications.

**Recommendation Generator** - Tailored, evidence-based intervention recommendations linked to assessment findings.

### Knowledge Base

- **Cognitive Assessment**: WISC-V administration, scoring, and interpretation guides
- **Behavioral Assessment**: Rating scale interpretation (BASC-3, Conners)
- **Emotional Assessment**: Anxiety and depression measure guides
- **Decision Trees**: Diagnostic pathways for LD, ADHD, and other conditions

## Workflow Example

```
# Start behavioral observation
/observe

# Calculate WISC-V scores
/score wisc-v SI:12 VC:11 BD:8 VP:7 MR:10 FW:9 DS:7 PS:6 CD:8 SS:7

# Interpret the profile
/interpret wisc-v VCI:106 VSI:81 FRI:96 WMI:78 PSI:83

# Explore differential diagnosis
/differential adhd-vs-anxiety

# Generate recommendations
/recommend working-memory-deficit processing-speed-weakness

# Draft report sections
/draft-section results
/draft-section recommendations

# Generate case summary
/case-summary
```

## Customization

### Personal Preferences

Create `.claude/CLAUDE.local.md` for your personal preferences:

```markdown
# My Assessment Preferences

## Report Style
- Strength-based language preferred
- Parent-friendly terminology

## Commonly Used Tests
- WISC-V, CTOPP-2, BASC-3, Beery VMI

## My Scoring Software
- Q-Interactive, Pearson online scoring
```

### Adding Knowledge

Add your own professional content to the `knowledge/` directory:
- Organize by domain (cognitive, emotional, behavioral)
- Use markdown format for easy reference
- Include examples and clinical guidelines

### Creating Custom Commands

Add custom slash commands to `.claude/commands/`:

```markdown
---
description: Your command description
---

Your command instructions here.
```

## Ethical Guidelines

This workspace enforces ethical guidelines:

1. **AI as Supplement** - All outputs require clinical review
2. **Confidentiality** - Use case numbers, not client names
3. **Scope of Practice** - AI supports, does not replace, clinical judgment
4. **Transparency** - Document AI assistance when appropriate

## Case Data Management

The `cases/` directory is gitignored for client confidentiality:
- Store all case data in `cases/`
- Use anonymized identifiers (Case001, Case002)
- Never commit client-identifying information

## Contributing

Contributions welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## License

MIT License - See LICENSE file for details.

## Disclaimer

This tool is designed to support licensed psychologists in their clinical work. It does not provide diagnoses or clinical decisions. All AI-generated content requires professional review and clinical judgment.

---

Built with [Claude Code](https://claude.ai/claude-code)
