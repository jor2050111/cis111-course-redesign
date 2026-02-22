# CIS111 Course Redesign - Claude Code Project Context

**Project Name:** CIS111 - Ethics in Information Technology Course Redesign
**Purpose:** Design and build a comprehensive, module-based course structure for CIS111 with OER-aligned content, learning objectives mapped to CLOs, and QM-aligned pedagogy
**Target Audience:** Community college students taking an introductory IT ethics course
**Course Format:** Online or hybrid (9-week accelerated or 16-week traditional)
**Sister Project:** [cis215-textbook](https://github.com/jor2050111/cis215-textbook) (shares pedagogical approach)

## Project Scope

This project is **not just an OER textbook**. It is a full course redesign that includes:

* **Module structure** defining what each of the 12 CIS111 modules should cover
* **Learning objectives** (MLOs) mapped to course learning outcomes (CLOs)
* **Content outlines** for instructional materials, case studies, and activities
* **Assessment design** including discussion prompts, quizzes, ethical analyses, and a capstone
* **OER content** where appropriate (readings, case studies, scenarios)

## Project Structure

```
cis111-course-redesign/
   CLAUDE.md                          # This file - project context
   README.md                          # Human-readable project overview
   .vscode/
      settings.json                 # Workspace settings
   modules/
      01-ethics-and-ethical-theories/
      02-professional-business-ethics/
      03-corporate-governance-csr-and-ai-ethics/
      04-social-media-responsibility/
      05-whistleblowing-and-accountability/
      06-healthcare-it-ethics/
      07-software-liability-and-secure-coding/
      08-government-regulation-and-self-regulation/
      09-intellectual-property-and-fair-use/
      10-freedom-of-expression-and-workplace-privacy/
      11-cybersecurity-identity-theft-and-risk-assessment/
      12-professional-ethics-and-capstone/
   assets/
      images/
         screenshots/
         diagrams/
      case-studies/
   templates/
      module-template.md
   docs/
      CIS111_CLOs.md                # Official CLOs and course outline
      module-structure.md           # 12-module structure with CLO mapping
      style-guide.md                # Writing and formatting standards
      blooms-taxonomy-reference.md  # Learning objective guidelines
```

## Critical Writing Standards

### MODULE LENGTH AND SCOPE

**This is an introductory ethics course. Each module should be focused and achievable in one week.**

**Course Structure:**
* **12 modules** organized into 4 thematic Parts
* Adaptable to 9-week accelerated (paired modules) or 16-week traditional format

**Module Content Guidelines:**
* 4-5 main sections (H2 headings) maximum
* 2-3 subsections (H3) per main section
* 1-2 case studies or ethical scenarios per module
* 2-3 discussion prompts per module
* Content should be readable in 1-2 hours (not including activities)

### Voice and Tone
* **Voice:** Second person ("you") for direct engagement
* **Tone:** Thoughtful, accessible, professional but not stiff
* **Technical level:** No prior ethics or IT background assumed
* **Avoid:** Academic passive voice, overly abstract philosophical language

### Module Structure Requirements (QM-Aligned)

Every module MUST follow this structure:

1. **Module Title** (H1) - `# Module N: [Title]`
2. **Narrative Introduction** - 2-3 engaging paragraphs setting context with a real-world hook
3. **Module Overview** - Time estimate, prerequisites, deliverables (QM Standard 3)
4. **Learning Objectives** - 2-3 MLOs with decimal numbering and RBT tags
5. **Main Content Sections** - 4-5 numbered sections (N.1, N.2, etc.) with:
   * **Case Study** or **Ethical Scenario** activities (at least 1 per module)
   * **Think About It** reflection prompts (2-3 per module)
   * **Quick Checks** (2-3 retrieval questions after each major section)
6. **Skills Lab** - Ethical analysis activity with rubric
7. **Summary and Retrieval** - Key concepts + Key Terms list + Retrieval Practice prompts
8. **Discussion Prompt** - Structured discussion question for online forums
9. **Further Reading** - 3-6 external resources (OER preferred)
10. **Looking Ahead** - 2-3 sentences previewing next module

### Learning Objectives Format

**Requirements:**
* 2-3 Module Learning Objectives (MLOs) per module
* Each MLO explicitly maps to one or more CLOs
* Use Bloom's Taxonomy action verbs
* Progression from lower to higher cognitive levels across the course
* Format: `**N.X-LOY (Bloom's Level):** [Verb] [measurable outcome] (CLO Z)`

**Example:**
```markdown
## Learning Objectives 🎯
By the end of this module, you will be able to:
* **1.1-LO1 (Understand):** Explain the core principles of utilitarianism, deontology, and virtue ethics (CLO I)
* **1.2-LO2 (Apply):** Apply ethical frameworks to analyze a real-world IT scenario (CLO I, II)
* **1.3-LO3 (Analyze):** Compare how different ethical theories lead to different conclusions about the same IT dilemma (CLO I)
```

### Module Overview (QM Standard 3)

Every module must include a Module Overview section:

```markdown
## Module Overview 🧭
* **Estimated time:** 4-5 hours (reading + activities + discussion)
* **Prerequisites:** None (Module 1) / Modules 1-2 (Module 3)
* **Deliverables:** Discussion post, Quick Checks, Skills Lab reflection
* **CLOs addressed:** CLO I, CLO II
```

### Decimal Section Numbering

**All main content sections use decimal numbering: N.1, N.2, N.3, etc.**

**Reserved section numbers:**
* N.1 through N.4: Main content sections
* N.5: Skills Lab (always)
* N.6: Summary and Retrieval (always)
* N.7: Discussion Prompt (always)

### Case Studies and Ethical Scenarios

**Critical pedagogical component for an ethics course.**

**Format:**
```markdown
### Case Study N.X - [Title]

**The Situation:** [2-3 paragraph real-world scenario]

**Stakeholders:** [List key parties involved]

**Questions to Consider:**
1. [Ethical analysis question]
2. [Stakeholder perspective question]
3. [What would you do? question]
```

**Guidelines:**
* Use real or realistic scenarios (with names changed if needed)
* Include multiple stakeholder perspectives
* Avoid scenarios with obvious "right answers"
* Connect to current events when possible
* Ensure diverse representation in scenarios

### Think About It Prompts

**Reflective pauses embedded throughout content:**

```markdown
> **Think About It:** [Reflection question connecting content to student experience]
```

**Guidelines:**
* Quick reflection (1-2 minutes)
* Connect abstract concepts to student's life or work experience
* No single correct answer
* Encourage personal ethical reasoning

### Heading Icons (REQUIRED for ALL modules)

```markdown
## Module Overview 🧭
## Learning Objectives 🎯
### Case Study N.X - [Title] 📋
### Think About It 💭
### Quick Check N.X ✅
## N.5 Skills Lab NA - [Title] (NO ICON)
## N.6 Summary and Retrieval 💡
## N.7 Discussion Prompt 💬
## Further Reading 📖
## Looking Ahead ⏩
```

### Lists
* **CRITICAL: Always use asterisks (`* `) for bullet points, NEVER dashes (`- `)**
* Use parallel structure (all items same grammatical form)

### Terminology Consistency

**Standard terms (use these exact forms):**
* IT (not "I.T." or "it" when referring to Information Technology)
* cybersecurity (one word, not "cyber security")
* internet (lowercase, per AP style)
* email (no hyphen)
* whistleblower (one word, no hyphen)
* healthcare (one word)
* open source (two words as noun/adjective, no hyphen)

## CLO-to-Module Quick Reference

| CLO | Module(s) |
|-----|-----------|
| I | 1 |
| II | 2 |
| III | 3 |
| IV | 4 |
| V | 5 |
| VI | 6 |
| VII | 5 |
| VIII | 7 |
| IX | 7 |
| X | 8 |
| XI | 9 |
| XII | 10 |
| XIII | 10 |
| XIV | 11 |
| XV | 11 |
| XVI | 11 |
| XVII | 12 |
| XVIII | 11 |

## Reference Files

**Always consult these files:**
* `/templates/module-template.md` - Module structure template
* `/docs/style-guide.md` - Writing and formatting standards
* `/docs/CIS111_CLOs.md` - Official course learning outcomes
* `/docs/module-structure.md` - 12-module organization with CLO mapping
* `/docs/blooms-taxonomy-reference.md` - Learning objective guidance

## Quality Checklist

Before considering a module complete, verify:

**Structure & Organization:**
* [ ] Decimal numbering used for all main sections (N.1, N.2, etc.)
* [ ] Module Overview includes time/prerequisites/deliverables/CLOs
* [ ] Narrative introduction (2-3 paragraphs) sets context with real-world hook
* [ ] "Looking Ahead" preview of next module included
* [ ] Heading hierarchy correct (no skipped levels)
* [ ] Heading icons present on all required sections

**Learning Objectives:**
* [ ] 2-3 MLOs with decimal numbering and RBT tags
* [ ] Each MLO explicitly references CLO(s) it addresses
* [ ] Bloom's taxonomy verbs used correctly
* [ ] Appropriate cognitive level for course progression

**Pedagogical Components:**
* [ ] At least 1 Case Study or Ethical Scenario per module
* [ ] 2-3 "Think About It" reflection prompts embedded in content
* [ ] Quick Checks after each major section (2-3 questions each)
* [ ] Skills Lab with ethical analysis activity and rubric
* [ ] Discussion Prompt with structured guidelines

**Content Quality:**
* [ ] Second-person voice ("you") used throughout
* [ ] Real-world examples and current events referenced
* [ ] Multiple stakeholder perspectives represented
* [ ] No overly simplistic "right/wrong" framing of ethical dilemmas
* [ ] Terminology consistent with style guide

**Summary & Assessment:**
* [ ] Summary includes Key Concepts + Key Terms + Retrieval Practice
* [ ] Discussion Prompt encourages ethical reasoning, not just opinion
* [ ] Further Reading has 3-6 curated OER resources
* [ ] Module length appropriate (readable in 1-2 hours)

## Task Management Preference

Use the **Tasks system** (TaskCreate, TaskUpdate, TaskList, TaskGet) for all project tracking and work coordination. Do NOT use the deprecated TodoWrite tool.

**When to create Tasks:**

* Before starting any multi-step work, break the work into Tasks with explicit dependencies.
* When spinning up subagents, create a shared Task list so all agents see current status.
* When a request involves changes across multiple files or modules, decompose into dependent Tasks first.

**How to structure Tasks:**

* Give each Task a clear, specific subject that describes a single deliverable.
* Set dependencies using `addBlockedBy` so Tasks execute in the correct order.
* Group independent Tasks together so subagents can work on them in parallel.
* Update Task status as you complete work. Mark Tasks done before moving to the next.

**Multi-session coordination:**
When working on a project that spans multiple sessions or subagents, use the shared Task list via the `CLAUDE_CODE_TASK_LIST_ID` environment variable. Store Tasks in `~/.claude/tasks/` so they persist across restarts.

**What NOT to do:**

* Do not use TodoWrite. It is deprecated and session-scoped only.
* Do not track work in your head or in conversational context alone. Create Tasks.
* Do not start implementation before defining the Task dependency chain for complex work.

## Banned Words/Phrases

Never use: spot-on, indeed, delve, dive, embark, nuances, journey, tapestry, navigate, em dashes

## Project Goals

**Primary objective:** Create a well-structured, QM-aligned course redesign for CIS111 that maps all 18 CLOs to focused modules with clear learning objectives, engaging case studies, and authentic assessments.

**Success criteria:**
* All 18 CLOs mapped to specific modules with traceable MLOs
* QM-aligned module structure with research-backed pedagogy
* Consistent voice and structure across all 12 modules
* Engaging case studies using real-world IT ethics scenarios
* Measurable learning objectives with explicit CLO alignment
* Active learning through case studies, reflections, and discussions
* OER-friendly content (no reliance on commercial textbook)

---

**Remember:** This file has higher authority than chat prompts. When in doubt, refer back to these standards. Consistency across modules is critical for student success.
