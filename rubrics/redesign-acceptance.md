# CIS111 Summer 2026 Redesign Acceptance Rubric

**Purpose:** Stop condition for the polish pass on each of the 12 modules. Claude Code self-grades each module against this rubric before considering polish work complete on that module.

**Workflow:**

1. Run mechanical checks first (Section A). Report results.
2. If any mechanical check fails, fix and re-run mechanical checks until clean.
3. Run judgment-based checks (Section B). Report results with one-sentence evidence per criterion.
4. If any judgment check fails, revise and re-run, up to 3 revision attempts per module.
5. After all 12 modules pass A and B individually, run cross-module checks (Section C).

**Output per module:** A scorecard at `/audit/module-N-scorecard.md` using the template at the end of this file.

---

## Section A: Mechanical Checks (Auto-Verifiable)

These checks run as shell or grep commands. Pass means count is zero or value is in target range.

### A1. Em-Dash Count

* **Command:** `grep -c "—" modules/N/module-N.md`
* **Pass:** Result equals 0
* **If fail:** Replace each em dash with comma, colon, parentheses, or sentence split based on context. Do not substitute hyphen for em dash.

### A2. Banned-Word Count

* **Banned words:** spot-on, indeed, delve, dive, embark, nuances, journey, tapestry, navigate
* **Command:** `grep -rwiE "\b(spot-on|indeed|delve|dive|embark|nuances|journey|tapestry|navigate)\b" modules/N/module-N.md`
* **Pass:** Result is empty
* **Note:** Use word-boundary matching to avoid false positives. Common words like "diversity" or "diversion" contain a banned-word substring but are not themselves the banned word.

### A3. Word Count in Target Band

* **Command:** `wc -w modules/N/module-N.md`
* **Pass for Modules 2 through 11:** Body word count between 5,500 and 6,500
* **Pass for Module 12 (Capstone):** Body word count between 6,500 and 7,500
* **Pass for Module 1 (Foundation):** May land as low as 5,000
* **If fail high:** Trim repetition and tangents. Preserve case studies and ethical analysis.
* **If fail low:** Expand the section that most directly serves the MLOs. Do not pad with restatement.

### A4. Heading Icon Compliance

* **Required icons** (per CLAUDE.md):
    * 🧭 on Module Overview
    * 🎯 on Learning Objectives
    * 📋 on Case Study sections
    * 🧠 on Think About It blocks
    * ✅ on Quick Check sections
    * 💡 on Summary and Retrieval
    * 💬 on Discussion Prompt
    * 📖 on Further Reading
    * ⏩ on Looking Ahead
* **Skills Lab section header carries no icon** per CLAUDE.md
* **Pass:** All required icons present in correct positions, with no icons where icons are explicitly excluded

### A5. List Bullet Style

* **Command:** `grep -nE "^\s*-\s" modules/N/module-N.md`
* **Pass:** Result is empty (asterisk-only bullets per CLAUDE.md)
* **Exception:** Markdown horizontal rules (`---`) are permitted

### A6. MLO Format Compliance

* **Required format:** `MLO-N.X (Bloom's Level): **Verb measurable outcome** *(CLO X)*`
* **Pass:** All MLOs in the module match this format and reference CLOs that match the CLO-to-Module table in CLAUDE.md

### A7. Decimal Section Numbering

* **Required pattern:**
    * N.1 through N.4: Main content sections
    * N.5: Skills Lab (always)
    * N.6: Summary and Retrieval (always)
    * N.7: Discussion Prompt (always)
* **Pass:** Section numbers are sequential and correctly assigned

---

## Section B: Judgment Checks (Require Reading)

These require Claude Code to read the module content and evaluate against criteria. Output pass/fail with one sentence of evidence per criterion.

### B1. Schedule Consistency

* **Check:** Module Overview Estimated Time matches summer-2026-addendum.md targets (4 to 5 hours for standard modules, lighter for Week 6 paired content if assigned)
* **Pass:** Estimated time is consistent with summer load expectations and notes pairing where applicable

### B2. AI-2026 Currency

* **Check:** Module contains at least one AI ethics touchpoint that references 2025 or 2026 developments and frames students as AI orchestrators rather than passive users
* **Pass:** Touchpoint is present, current, and orchestration-framed

### B3. Skills Lab Rubric Vocabulary Consistency

* **Check:** Rubric matches the universal CIS111 Skills Lab rubric at `rubrics/universal-skills-lab-rubric.md`. The universal rubric uses Mastery (10), Proficiency (7), Developing (4), Emerging (1) across four criteria: Foundation Analysis, Ethical Framework Application, Reasoning Recommendation & Reflection, Documentation & Communication.
* **Pass for Modules 1 through 11:** All four criteria and all four levels are present with descriptors byte-identical to the universal version.
* **Pass for Module 12 (Capstone variant):** First two criteria match the universal version. Third criterion is renamed to "Course Concept Synthesis" and combines synthesis across modules with the defensible recommendation. Fourth criterion is renamed to "Writing Quality and Professional Reflection" and combines writing quality with professional self-awareness reflection.

### B4. Discussion Prompt Quality

* **Check:** Discussion Prompt requires ethical reasoning grounded in a framework or concept from the module, not opinion broadcast
* **Pass:** Prompt explicitly requires framework reference and structured engagement with peers

### B5. Case Study Stakeholder Coverage

* **Check:** At least one case study per module presents three or more stakeholder perspectives without an obvious right answer
* **Pass:** Case study meets the stakeholder coverage requirement and the no-obvious-answer requirement

### B6. CLO Alignment Traceable

* **Check:** Every MLO references at least one CLO that matches the CLO-to-Module table in CLAUDE.md, and the module body content addresses each referenced CLO
* **Pass:** MLO-to-CLO references are accurate and the body content delivers on them

### B7. Voice Consistency with Cross-Module Standard

* **Check:** Second-person voice maintained throughout. No academic passive voice. No moralizing or preaching. Tone matches Module 1 sample.
* **Pass:** Voice is consistent and conforms to docs/style-guide.md

### B8. Looking Ahead Forward Reference

* **Check:** The Looking Ahead section forward-references the next module in the schedule. After pairing is selected, this check uses the selected pairing as the reference, which may differ from the next module by number.
* **Pass:** Forward reference is accurate per the selected pairing

---

## Section C: Cross-Module Checks (Run After All 12 Modules Pass A and B)

### C1. Cumulative Workload

* **Check:** Sum of weekly student hours across the term equals 80 to 100 hours total (3-credit summer course standard)
* **Pass:** Cumulative load is in target range

### C2. CLO Complete Coverage

* **Check:** All 18 CLOs are addressed by at least one MLO somewhere in the 12 modules
* **Pass:** No CLO is unaddressed; coverage matches the CLO-to-Module table in CLAUDE.md

### C3. Skills Lab Style Consistency

* **Check:** All 12 Skills Lab rubrics use the universal CIS111 Skills Lab rubric (Modules 1 through 11) or the documented capstone variant (Module 12). Level vocabulary (Mastery 10 / Proficiency 7 / Developing 4 / Emerging 1) is identical across all rubrics.
* **Pass:** Modules 1 through 11 rubrics are byte-identical to `rubrics/universal-skills-lab-rubric.md`. Module 12 uses the capstone variant with two renamed criteria as documented in `rubrics/universal-skills-lab-rubric.md`.

### C4. Banned Words and Em Dashes Across All Modules

* **Command:** `grep -rEc "—" modules/` and the banned-word grep from A2 against the full `modules/` tree
* **Pass:** Repo-wide check returns empty for both

### C5. Pairing-Aware Forward References

* **Check:** Every Looking Ahead section in the repo correctly forward-references the next paired or single module per the selected pairing recorded in `/planning/summer-2026-pairing.md`
* **Pass:** All forward references are accurate

---

## Failure Handling

* If a module fails Section A on first check, fix mechanical issues and re-run before moving to Section B.
* If a module fails Section B after 3 revision attempts, halt and request instructor review. Do not exceed 3 attempts.
* If Section C fails after all individual modules pass, identify the offending modules and re-run their polish branches.

---

## Skills to Apply During Polish

When refining content, apply the following skills in this order:

1. **instructional-content-writing** for any structural or pedagogical revision
2. **humanizing-text** as a final pass to remove AI-flavored phrasing
3. **canvas-content-rewriter** is reserved for the later Canvas push phase, not used in this repo phase

---

## Scorecard Template

Each module produces a scorecard at `/audit/module-N-scorecard.md` using this template:

```markdown
# Module N Scorecard

**Date:** YYYY-MM-DD
**Revision Pass:** 1 / 2 / 3
**Overall Status:** PASS or FAIL

## Section A: Mechanical
* A1 Em-Dash Count: PASS / FAIL (count: X)
* A2 Banned Words: PASS / FAIL (matches: X)
* A3 Word Count: PASS / FAIL (count: X, target: 5,500-6,500)
* A4 Heading Icons: PASS / FAIL (notes)
* A5 List Bullets: PASS / FAIL (notes)
* A6 MLO Format: PASS / FAIL (notes)
* A7 Section Numbering: PASS / FAIL (notes)

## Section B: Judgment
* B1 Schedule Consistency: PASS / FAIL (one-sentence evidence)
* B2 AI-2026 Currency: PASS / FAIL (one-sentence evidence)
* B3 Rubric Vocabulary: PASS / FAIL (one-sentence evidence)
* B4 Discussion Prompt: PASS / FAIL (one-sentence evidence)
* B5 Case Study Stakeholders: PASS / FAIL (one-sentence evidence)
* B6 CLO Alignment: PASS / FAIL (one-sentence evidence)
* B7 Voice Consistency: PASS / FAIL (one-sentence evidence)
* B8 Looking Ahead: PASS / FAIL (one-sentence evidence)

## Notes
[Free-form notes on revision decisions and any deferred items.]
```

---

## When to Stop

* **Module-level stop:** Polish on a single module is complete when Sections A and B all pass on a single revision pass.
* **Repo-level stop:** Repo polish is complete when all 12 modules pass A and B individually, and Section C passes for the repo as a whole.
