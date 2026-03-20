# CIS111 Course Redesign - Style Guide

## Writing Standards

### Voice and Tone

* **Voice:** Second person ("you") for direct engagement
* **Tone:** Thoughtful, accessible, professional but conversational
* **Level:** Accessible to students with no prior ethics or IT background
* **Approach:** Present ethical dilemmas fairly; avoid preaching or moralizing
* **Avoid:** Academic passive voice, overly abstract philosophical jargon, condescending language

### Presenting Ethical Issues

* **Always present multiple perspectives** on controversial topics
* **Avoid taking sides** in ethical debates; guide students to form their own conclusions
* **Use precise language** when describing legal and ethical concepts
* **Distinguish clearly** between what is legal, what is ethical, and what is common practice
* **Acknowledge complexity** without being vague or wishy-washy

### Inclusive Language

* Use gender-neutral language (they/them for hypothetical individuals)
* Include diverse names and backgrounds in case studies and scenarios
* Represent diverse industries and organizational sizes
* Avoid assumptions about students' technical background or work experience

---

## Formatting Standards

### Heading Hierarchy

* **H1:** Module title only (`# Module N: [Title]`)
* **H2:** Major sections with decimal numbering (`## N.1 [Topic]`)
* **H2:** Also used for Module Overview, Learning Objectives, Skills Lab, Summary, Discussion
* **H3:** Subsections, Case Studies, Quick Checks, Think About It
* **Never skip heading levels**

### Heading Icons (Required)

```
## Module Overview 🧭
## Learning Objectives 🎯
### Case Study N.X - [Title] 📋
### Think About It 🧠      (or use blockquote format inline)
### Quick Check N.X ✅
## N.5 Skills Lab NA - [Title]  (NO ICON)
## N.6 Summary and Retrieval 💡
## N.7 Discussion Prompt 💬
## Further Reading 📖
## Looking Ahead ⏩
```

### Lists

* **CRITICAL: Always use asterisks (`* `) for bullet points, NEVER dashes (`- `)**
* Use parallel structure (all items same grammatical form)
* Use numbered lists for sequential steps or ranked items
* Use bullet lists for non-sequential collections

### Inline Formatting

* **Bold** for first mention of key terms
* *Italic* for emphasis and publication titles
* `Inline code` for specific technology names, commands, file names
* "Quotation marks" for direct quotes only

### Tables

* Use pipe tables for maximum compatibility
* Keep content concise within cells
* Left-align text columns, center-align short data

### Blockquotes

* Use for "Think About It" prompts:
  ```markdown
  > **Think About It:** 🧠 Your reflection question here
  ```
* Use for important callouts or notable quotes (with attribution)

---

## Content Standards

### Case Studies

* **Length:** 2-4 paragraphs for the scenario description
* **Realism:** Based on real events when possible (change names if needed)
* **Complexity:** Include genuine ethical tension with no obvious "right answer"
* **Stakeholders:** Always identify 3+ stakeholders with different interests
* **Questions:** 3 questions progressing from analysis to personal judgment
* **Currency:** Reference recent events when possible (within last 5 years)

### Discussion Prompts

* Require ethical reasoning, not just personal opinion
* Reference specific module concepts or frameworks
* Allow for respectful disagreement
* Include clear guidelines for post length and response expectations
* Avoid yes/no questions; use "to what extent" or "under what circumstances"

### Quick Checks

* 2-3 questions per check
* Mix of Remember and Understand levels
* Placed after each major content section
* Low-stakes, formative assessment
* Can be self-checked by students

### Skills Labs

* Single multi-part activity per module
* Progressive difficulty (Foundation, Application, Extension)
* Always include rubric with 5-level scale
* Align explicitly with MLOs
* Realistic scenarios or source materials

---

## Terminology

### Standard Terms (use exact forms)

| Correct | Incorrect |
|---------|-----------|
| IT | I.T., it (when meaning Information Technology) |
| cybersecurity | cyber security, cyber-security |
| internet | Internet (lowercase per AP style) |
| email | e-mail |
| whistleblower | whistle-blower, whistle blower |
| healthcare | health care, health-care |
| open source | open-source (as noun/adjective) |
| data breach | databreach |
| personally identifiable information (PII) | personal identifiable information |
| intellectual property (IP) | Intellectual Property (don't capitalize in running text) |

### Acronyms

* Spell out on first use in each module, followed by acronym in parentheses
* After first use, acronym alone is acceptable
* Exception: Extremely common acronyms (IT, AI, US) may be used without expansion

### Legal and Regulatory Terms

* Always use official names for laws and regulations on first mention
* Example: "the Health Insurance Portability and Accountability Act (HIPAA)"
* After first mention: "HIPAA" is sufficient
* Don't assume students know what any law does; briefly explain its purpose

---

## Citation and Attribution

### For OER Content

* Provide complete attribution per Creative Commons requirements
* Include: Title, Author, Source URL, License type
* Format: `[Title](URL) by [Author], licensed under [CC License]`

### For Case Studies Based on Real Events

* Clearly state that the scenario is "based on real events" or "inspired by" when applicable
* Change individual names if discussing non-public figures
* Include a "Learn More" link to the original reporting when appropriate

### For Statistics and Claims

* Always cite the source for specific statistics
* Prefer recent sources (within 5 years when possible)
* Use reputable sources (government data, academic research, major news outlets)

---

## Accessibility (WCAG 2.1 AA)

* All images must have descriptive alt text
* Don't rely on color alone to convey meaning
* Use descriptive link text (not "click here")
* Maintain clear heading hierarchy for screen readers
* Tables must have header rows
* Keep language at appropriate reading level (aim for 10th-12th grade)

---

## Banned Words/Phrases

Never use: spot-on, indeed, delve, dive, embark, nuances, journey, tapestry, navigate, em dashes

---

## File Naming Conventions

**Modules:** `module-[NN].md` (e.g., `module-01.md`)
**Images:** `mod[NN]-[description].png` (e.g., `mod01-ethical-frameworks-diagram.png`)
**Case Studies:** `case-[NN]-[short-name].md` (e.g., `case-01-facebook-cambridge-analytica.md`)
**Diagrams:** `mod[NN]-[description].png` in `assets/images/diagrams/`
