# Module 11 Scorecard

**Date:** 2026-05-07
**Revision Pass:** 1
**Overall Status:** PASS

## Section A: Mechanical

* A1 Em-Dash Count: PASS (count: 0)
* A2 Banned Words: PASS (matches: 0)
* A3 Word Count: PASS (count: 6,499, target 5,500-6,500)
* A4 Heading Icons: PASS (Module Overview 🧭, Learning Objectives 🎯, Case Study 📋, Think About It 🧠, Quick Check ✅, Summary 💡, Discussion 💬, Further Reading 📖, Looking Ahead ⏩; Skills Lab 11.5 carries no icon as required)
* A5 List Bullets: PASS (no hyphen bullets; all asterisks)
* A6 MLO Format: PASS (3 of 3 MLOs match `MLO-N.X (Bloom's): **Verb...** *(CLO X)*` format; reference CLOs XIV, XV, XVI, XVIII consistent with the CLO-to-Module table in CLAUDE.md; only Create-level MLO outside Module 12)
* A7 Section Numbering: PASS (11.1-11.7 sequential, 11.5 Skills Lab, 11.6 Summary, 11.7 Discussion)

## Section B: Judgment

* B1 Schedule Consistency: PASS — Module Overview Estimated Time is 5-6 hours, justified for the densest module in the course (4 CLOs, only Create-level MLO outside the capstone, large body of regulatory and technical content). Sits alone in W8 of Option 1 with no pairing partner, so the slightly elevated load fits the schedule.
* B2 AI-2026 Currency: PASS — Section 11.4 now contains a "2025-2026 Snapshot" subsection covering autonomous-triage AI maturation through 2025, 2025 adversarial-input attacks against commercial AI detectors, EU AI Act high-risk classification of critical-infrastructure AI phasing in through 2025-2026, and CISA's 2025 secure-by-design guidance plus updated NIST AI RMF profiles. Three distinct 2025/2026 references; student framed as orchestrator-verifier of AI security platforms.
* B3 Skills Lab Rubric Vocabulary: PASS — Skills Lab 11A rubric uses Mastery (5), Proficiency (4), Developing (3), Emerging (2), Not Evident (1) across 5 criteria, matching the cross-module standard.
* B4 Discussion Prompt Quality: PASS — Prompt anchors on the 2024 Hong Kong deepfake $25M wire-fraud incident, requires students to take a position on employee accountability for AI social-engineering attacks, support it with at least two module concepts, and address the strongest counterargument; 250-350 words + 2 substantive peer responses.
* B5 Case Study Stakeholder Coverage: PASS — Case Study 11.1 (Anthem Healthcare Breach) presents 5 stakeholders (78.8 million members/employees, Anthem leadership/IT security team, healthcare providers/partners, federal/state regulators, broader healthcare industry) with competing interests and no obvious correct answer.
* B6 CLO Alignment: PASS — CLO XIV (identity theft) addressed in §11.2; CLO XV (security breaches and risk assessments) in §11.3; CLO XVI (security policies) in §11.3; CLO XVIII (prevention/detection/response) in §11.4. All 3 MLOs reference these CLOs; body content delivers on each.
* B7 Voice Consistency: PASS — Second-person ("you") sustained throughout. No academic passive voice. No moralizing. Tone matches Module 1 sample.
* B8 Looking Ahead: PASS — Looking Ahead forward-references Module 12. Under selected Option 1, M11 (W8 single) is followed by M12 (W9 capstone). Forward reference is accurate for the selected pairing.

## Notes

**Trim summary.** Reduced from 8,530 to 6,499 words (2,031 words / 23.8%). The trim was the heaviest of the three completed modules so far, driven by M11's pre-polish density: 4 CLOs, the only Create-level MLO outside the capstone, and substantial regulatory and technical reference content. Cuts targeted (1) restated section openers, (2) "first/second/third" enumerated explanations where the bullet structure already conveys enumeration, (3) repeated definitions of CIA Triad terms after their initial introduction, (4) parallel-structure paragraphs in the CDSS-style "issues-with-X" sections, and (5) Key Concepts bullets in section 11.6 that paraphrased their own body text. Preserved in full per task spec: SolarWinds narrative hook, Case Study 11.1 (Anthem Healthcare Breach), Skills Lab 11A scenario (MidState Community College incident response plan) with its rubric, all Quick Checks and Think About It blocks, MLO statements, the Discussion Prompt with its 2024 Hong Kong deepfake anchor, and the exploits table.

**B2 addition.** Added a new H3 subsection "A 2025-2026 Snapshot: AI-vs-AI Defense and Critical-Infrastructure Rules" in section 11.4 between the Limitations bullets and Think About It 11.4. Approximately 130 words. Names two concrete 2025-2026 anchors (autonomous-triage AI in commercial SIEM/EDR through 2025; EU AI Act high-risk classification of critical-infrastructure AI plus CISA secure-by-design guidance and NIST AI RMF profiles) without naming specific vendors. The orchestrator-verifier frame mirrors M5 and M6 for cross-module consistency.

**Cross-module continuity.** M11 now extends the AI-2026 thread established in M5 (insider-risk and HR monitoring) and M6 (clinical AI regulation and ambient scribes). Across M5, M6, and M11 the orchestrator-verifier frame is consistent: AI outputs are inputs to human judgment, not substitutes for it. M11's contribution is the most operationally concrete (auto-triage closing alerts, containment actions) because cybersecurity is where AI is acting most autonomously today.

**Section C (cross-module) deferral.** Per task spec, this scorecard reports A and B only. C runs after all 12 modules pass A and B individually.

**Branch state.** `polish/module-11` contains three commits ahead of main:
1. `polish(module-11): mechanical pass` (Section A)
2. `polish(module-11): judgment pass` (Section B)
3. `polish(module-11): final scorecard, all rubric checks pass` (this file)

Branch will be pushed to remote upon final commit.
