# CIS111 - Ethics in Information Technology: Course Redesign

**A comprehensive course redesign for CIS111, building module structure, learning objectives, and OER content for an introductory IT ethics course.**

## Project Overview

This project redesigns CIS111 (Ethics in Information Technology) from the ground up, organizing the course into 12 focused modules that map to the 18 official Course Learning Outcomes (CLOs). The redesign follows Quality Matters (QM) standards and Revised Bloom's Taxonomy (RBT) for learning objective design.

Unlike a standalone textbook project, this redesign covers the full scope of course structure: what each module should teach, how learning objectives align to CLOs, what case studies and activities support learning, and how assessments measure student achievement.

### Target Audience

* Community college students
* No prior background in ethics or IT required
* Mix of IT majors and general education students
* Career-oriented and practical focus

### Key Topics Covered

* Ethical theories and frameworks (utilitarianism, deontology, virtue ethics)
* Corporate responsibility and governance
* Social media ethics and privacy
* Whistleblowing and accountability
* Healthcare IT ethics (HIPAA, mHealth)
* Software liability and secure coding
* Government regulation (GDPR, CCPA, COPPA)
* Intellectual property and fair use
* Freedom of expression, hate speech, and defamation
* Cybersecurity, identity theft, and risk assessment
* Professional codes of ethics (ACM, IEEE, (ISC)²)

## Project Structure

```
cis111-course-redesign/
├── CLAUDE.md                          # Claude Code project context (AI assistant guide)
├── README.md                          # This file
├── modules/
│   ├── 01-ethics-and-ethical-theories/
│   ├── 02-corporate-responsibility/
│   ├── 03-social-media-and-privacy/
│   ├── 04-whistleblowing-and-accountability/
│   ├── 05-software-liability-and-secure-coding/
│   ├── 06-government-regulation-and-self-regulation/
│   ├── 07-intellectual-property-and-fair-use/
│   ├── 08-freedom-of-expression-and-defamation/
│   ├── 09-privacy-and-workplace-monitoring/
│   ├── 10-cybersecurity-and-risk-assessment/
│   ├── 11-identity-theft-and-cybercrime/
│   └── 12-professional-ethics-and-codes-of-conduct/
├── assets/
│   ├── images/
│   │   ├── screenshots/
│   │   └── diagrams/
│   └── case-studies/
├── templates/
│   └── module-template.md
└── docs/
    ├── CIS111_CLOs.md                 # Official CLOs and course outline
    ├── module-structure.md            # 12-module structure with CLO mapping
    ├── style-guide.md                 # Writing and formatting standards
    └── blooms-taxonomy-reference.md   # Learning objective guidelines
```

## Getting Started

### Prerequisites

* VS Code with Claude Code extension installed
* Git (for version control)

### Initial Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/jor2050111/cis111-course-redesign.git
   ```

2. **Review foundation files:**
   * [CLAUDE.md](CLAUDE.md) - Project context for Claude Code
   * [docs/CIS111_CLOs.md](docs/CIS111_CLOs.md) - Course learning outcomes
   * [docs/module-structure.md](docs/module-structure.md) - Module organization
   * [templates/module-template.md](templates/module-template.md) - Module structure template

## Course Organization

### 12 Modules in 4 Parts

| Part | Modules | Theme |
|------|---------|-------|
| **I: Foundations of Ethics** | 1-3 | Ethical theories, business ethics, corporate responsibility |
| **II: Digital Rights and Responsibilities** | 4-6 | Social media, whistleblowing, healthcare IT |
| **III: Legal Frameworks and IT Obligations** | 7-9 | Software liability, regulation, intellectual property |
| **IV: Security, Privacy, and Professional Practice** | 10-12 | Speech/privacy, cybersecurity, professional codes |

### CLO Coverage

All 18 CLOs are mapped to specific modules. See [docs/module-structure.md](docs/module-structure.md) for the complete mapping table.

## Development Workflow

### Creating Module Content

1. **Review the module's CLO mapping** in `docs/module-structure.md`
2. **Use the module template** at `templates/module-template.md`
3. **Write learning objectives** using Bloom's Taxonomy (see `docs/blooms-taxonomy-reference.md`)
4. **Develop content** with case studies, ethical scenarios, and reflection prompts
5. **Create assessments** aligned to MLOs and CLOs

### Quality Checklist

Before finalizing a module:

* [ ] 2-3 MLOs with RBT tags and CLO references
* [ ] Module Overview with time estimate, prerequisites, deliverables
* [ ] At least 1 case study or ethical scenario
* [ ] Quick Checks after major sections
* [ ] Skills Lab with rubric
* [ ] Discussion Prompt
* [ ] Summary with Key Terms and Retrieval Practice
* [ ] Consistent second-person voice
* [ ] Heading icons present

## Relationship to CIS215 Textbook

This project shares pedagogical patterns with the [cis215-textbook](https://github.com/jor2050111/cis215-textbook) project:

* QM-aligned module/chapter structure
* Decimal section numbering (N.1, N.2, etc.)
* Bloom's Taxonomy learning objectives with RBT tags
* Quick Checks for spaced retrieval practice
* Skills Labs with rubrics
* Consistent heading icon system

**Key differences from CIS215:**
* Focus on ethics and critical thinking rather than technical skills
* Case studies and ethical scenarios replace code examples
* Discussion prompts replace coding exercises
* "Think About It" reflections replace "Try It Yourself" coding activities
* Content is conceptual/analytical rather than procedural

## License

CC BY-NC-SA 4.0 (Creative Commons Attribution-NonCommercial-ShareAlike 4.0)

## Contact

Mr. Vega (Jorge) - IT Faculty, Phoenix College
Jorge.Vega@PhoenixCollege.edu

---

**Last Updated:** February 2026

**Status:** Initial Setup / Active Development
