# Polish Task: Module 11 (Cybersecurity, Identity Theft, and Risk Assessment)

**Module:** 11-cybersecurity-identity-theft-and-risk-assessment
**Working file:** `modules/11-cybersecurity-identity-theft-and-risk-assessment/module-11.md`
**Branch:** `polish/module-11`
**Output scorecard:** `/audit/module-11-scorecard.md`
**Authority for stop-condition:** `rubrics/redesign-acceptance.md`

---

## Why Module 11 Next

Module 11 is the third polish target because:

* It is the heaviest standalone module by word count (8,530), the most CLO-dense (CLOs XIV, XV, XVI, XVIII), and carries the only Create-level MLO outside the capstone. Polishing it now removes the largest remaining trim job from the queue.
* Under selected Option 1 (Theme-Density), M11 sits alone in Week 8 between the M9+M10 paired week and the M12 capstone. It has no pairing partner, so polishing it is independent of any other module's pacing.
* B2 will fail: M11 has zero 2025/2026 references at audit time. The cybersecurity-AI angle is rich for currency: AI-assisted attacks, AI-driven SOC operations, deepfake-enabled fraud, and 2025-2026 ransomware/identity-theft developments.
* Trim is heavier than M5 and M6 (~26% reduction needed). Apply the same pattern: preserve case studies, Quick Checks, Skills Lab, MLOs, and narrative hook; trim restated section openers, repeated definitions, and connective tissue.

---

## Pre-Flight

```bash
git checkout main
git pull
git checkout -b polish/module-11
mkdir -p audit
```

---

## Reading Order

1. `CLAUDE.md`
2. `docs/summer-2026-addendum.md` (length targets, AI-2026 currency requirement)
3. `planning/summer-2026-pairing.md` (Option 1 selected; M11 alone in W8)
4. `rubrics/redesign-acceptance.md`
5. `docs/style-guide.md`
6. `docs/CIS111_CLOs.md` (CLOs XIV, XV, XVI, XVIII full text)
7. `templates/module-template.md`
8. `modules/11-cybersecurity-identity-theft-and-risk-assessment/module-11.md`
9. `audit/module-05-scorecard.md` and `audit/module-06-scorecard.md` (reference)

---

## Workflow

### Step 1: Mechanical Audit (Section A)

Run all Section A checks. Report counts. Output preliminary results to `/audit/module-11-scorecard.md`.

### Step 2: Mechanical Fixes

* **A3 (word count):** Trim from 8,530 to ~6,300-6,400 (mid-band, with B2 headroom). Same preserve/trim guidance as M5 and M6 polish tasks.
* **A1, A2, A4-A7:** apply mechanical fixes per CLAUDE.md and the rubric.

After mechanical fixes, re-run Section A. All items must PASS.

**Commit:** `polish(module-11): mechanical pass (trim, banned-word check, format compliance)`

### Step 3: Judgment Audit (Section B)

Run all Section B checks. Report one-sentence evidence per criterion.

* B1 Schedule Consistency (4-5 hours; M11 is a single in W8 of Option 1)
* B2 AI-2026 Currency (will fail; add a current touchpoint)
* B3-B7: Skills Lab rubric, discussion prompt quality, case study stakeholder coverage, CLO alignment for CLOs XIV/XV/XVI/XVIII, voice consistency
* B8 Looking Ahead (Option 1 selected: M11 followed by M12 in W9; verify forward reference)

### Step 4: Judgment Revisions

For B2, suggested 2025-2026 angles in section 11.4 (Incident Response, Computer Forensics, and AI in Cybersecurity):

* AI-augmented social engineering and spear-phishing at scale across 2024-2025, with documented incidents using cloned voices and AI-generated emails
* AI-powered SOC platforms and detection systems maturing through 2025
* Deepfake-enabled fraud incidents reported in 2024-2025
* CISA / NIST AI Risk Management Framework and the EU AI Act's high-risk classification for AI used in critical infrastructure
* The shift toward "AI vs AI" cybersecurity in 2025-2026 (defenders using AI to detect AI-generated attacks)

Frame the IT professional as orchestrator-verifier of AI security tools, not passive consumer of AI alerts. Connect to existing CIA Security Triad content, since accountability for AI-driven security decisions hits Confidentiality, Integrity, and Availability differently.

After revisions, re-run Section B. All must PASS.

**Commit:** `polish(module-11): judgment pass (AI-2026 currency, voice, CLO alignment)`

### Step 5: Iteration Limit

* Maximum 3 revision passes total
* If after 3 passes any criterion fails, halt and write halt notes to scorecard

### Step 6: Final Scorecard and Commit

* Update `/audit/module-11-scorecard.md` with final PASS/FAIL per criterion
* Final commit: `polish(module-11): final scorecard, all rubric checks pass`
* Push branch to remote.

---

## Stop Conditions

* Stop when all Section A and Section B criteria pass on a single revision pass
* OR stop after 3 revision passes
* This task is module-11 only; do not modify other modules

---

## Expected Output

1. Modified `modules/11-cybersecurity-identity-theft-and-risk-assessment/module-11.md` (trimmed from ~8,530 to ~6,400 words; 2025-2026 cybersecurity-AI touchpoint added)
2. New `/audit/module-11-scorecard.md`
3. Three commits on `polish/module-11` branch
4. Branch pushed to remote, ready for PR review
