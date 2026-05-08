# Module 4 Scorecard

**Date:** 2026-05-07
**Revision Pass:** 1
**Overall Status:** PASS

## Section A: Mechanical

* A1 Em-Dash Count: PASS (count: 0)
* A2 Banned Words: PASS (matches: 0; none of spot-on, indeed, delve, dive, embark, nuances, journey, tapestry, navigate detected)
* A3 Word Count: PASS (count: 6,248, target: 5,500-6,500; pre-polish was 5,615, expanded to 6,248 via B2 additions)
* A4 Heading Icons: PASS (Module Overview 🧭, Learning Objectives 🎯, Think About It 4.1/4.3/4.4 🧠, Quick Check 4.1/4.2/4.3/4.4 ✅, Case Study 4.1 📋, Summary and Retrieval 💡, Discussion Prompt 💬, Further Reading 📖, Looking Ahead ⏩; Skills Lab 4.5 carries no icon as required)
* A5 List Bullets: PASS (no hyphen bullets; all asterisks)
* A6 MLO Format: PASS (3 of 3 MLOs match `MLO-N.X (Bloom's Level): **Verb measurable outcome** *(CLO X)*` format; all three reference CLO IV, consistent with the CLO-to-Module table in CLAUDE.md)
* A7 Section Numbering: PASS (4.1-4.7 sequential; 4.5 Skills Lab, 4.6 Summary and Retrieval, 4.7 Discussion Prompt)

## Section B: Judgment

* B1 Schedule Consistency: PASS — Module Overview Estimated Time is 4-5 hours, appropriate for a standard single module; M4 is alone in W3 (June 8-14) under Option 1, so the standard load estimate is correct.
* B2 AI-2026 Currency: PASS — New deepfakes paragraph anchors to 2024-2025 U.S. political deepfake incidents and state disclosure laws (18+ states by early 2025); new subsection "Platform AI in 2025-2026: Regulation, Disclosure, and Your Role as Verifier" introduces EU DSA enforcement (2024-2025), EU AI Act high-risk classification for recommendation systems, and the orchestrator-verifier frame with direct second-person application; orchestrator-verifier added to Key Terms; Key Concepts updated with 2024-2025 regulatory anchor; Discussion Prompt updated to reference DSA alongside 2024-2025 U.S. state laws.
* B3 Rubric Vocabulary: PASS — Skills Lab 4A rubric uses Mastery (5), Proficiency (4), Developing (3), Emerging (2), Not Evident (1) across 5 criteria (Stakeholder Analysis, Ethical Framework Application, Module Concept Application, Recommendation Quality, Writing and Professionalism), matching the cross-module standard.
* B4 Discussion Prompt Quality: PASS — Updated prompt requires students to take and defend a position on whether government mandate (age verification or algorithmic risk assessment) or platform self-regulation is sufficient, referencing at least one ethical framework and addressing the strongest counterargument using a different framework; framework reference and structured peer engagement are explicitly required.
* B5 Case Study Stakeholders: PASS — Case Study 4.1 (StreamView Recommendation Engine Dilemma) presents 5 stakeholder groups (leadership/shareholders, users, advertisers, content moderators, society at large) with genuinely competing interests; no obvious correct answer because the financial cost of algorithm change is real ($400M estimated) and the ethical obligation to act on internal research is equally real.
* B6 CLO Alignment: PASS — CLO IV (Social media responsibility) is traced through all four content sections: §4.1 covers data collection and informed consent (MLO-4.1 Understand), §4.2 covers content moderation and algorithmic bias (MLO-4.3 Analyze), §4.3 covers hiring and cyberabuse (MLO-4.2 Apply), §4.4 covers attention economy, deepfakes, and AI recommendation systems including 2025-2026 regulatory context (MLO-4.2/4.3 Apply/Analyze); all three MLOs reference CLO IV correctly.
* B7 Voice Consistency: PASS — Second-person ("you") sustained throughout all content sections including the new AI touchpoint subsection ("You are not a passive recipient of whatever a recommendation algorithm delivers," "When you use social media, you can exercise the role of orchestrator and verifier"); no academic passive voice; no moralizing; direct and action-oriented phrasing consistent with the M1/M3/M5 cross-module standard.
* B8 Looking Ahead: PASS — Looking Ahead correctly forward-references Module 5 (Whistleblowing and Accountability); under selected Option 1, M4 is alone in W3 and M5+M6 are paired in W4, so forward-referencing M5 is accurate per the binding schedule.

## Notes

**Pre-polish module was mechanically clean.** No A-check failures required remediation. The first commit captured both the mechanical pass verification and the B2 additions (consistent with M1 scorecard precedent where B2 additions were staged before the first commit).

**B2 additions: placement rationale.** Two additions were made. First, the existing "Deepfakes and Synthetic Media" subsection was strengthened with a 2024-2025 paragraph covering U.S. political deepfake incidents during the 2024 election cycle, state disclosure laws (18+ states by early 2025), and platform labeling efforts. Second, a new subsection "Platform AI in 2025-2026: Regulation, Disclosure, and Your Role as Verifier" was added at the end of §4.4 between "AI Recommendation Systems and Autonomy" and Quick Check 4.4. This location is pedagogically correct: students have just read about recommendation algorithm harms, and the new subsection shows them the regulatory response to those harms and frames their own critical engagement as an ethical practice. Placement after the autonomy discussion and before the Quick Check follows the same three-point anchoring pattern used in M1 and M3.

**Orchestrator-verifier introduction.** M4 is the first module in the course where students directly encounter platform AI as a system acting on them (recommendation algorithms, deepfake generation). The orchestrator-verifier frame is therefore introduced here in a user-facing context: you can verify algorithmic output, choose non-personalized feeds, and cross-check sources. This complements the M3 governance-level introduction of the concept (companies must govern AI systems) and the M1 foundation-level introduction (four ethical frameworks are reasoning tools for the orchestrator-verifier role). M5 will extend the frame to internal whistleblowing contexts where AI compliance tools may flag or suppress employee behavior.

**EU DSA and AI Act references.** The DSA enforcement timeline (2024 formal proceedings) and EU AI Act high-risk classification for recommendation systems are grounded in the actual regulatory trajectory as of 2025. These references satisfy B2's requirement for 2025-2026 currency and connect to the M3 AI governance anchor without duplicating M3's full treatment of the EU AI Act. The M3 reference in the new subsection ("the M3 principles of fairness, transparency, and human oversight") is the explicit backward reference called for in the workflow instructions.

**Discussion Prompt update.** The pre-polish prompt was anchored to 2024 U.S. state age verification laws only. The updated prompt adds the EU DSA as a parallel regulatory approach, broadens the question from age verification specifically to platform accountability mechanisms generally (which includes algorithmic risk assessment), and frames the regulatory debate more accurately as a 2024-2025 ongoing development rather than a resolved question. The structural requirements (take a position, use one framework, address strongest counterargument with a different framework) remain unchanged.

**B8 forward reference confirmed.** Looking Ahead points to M5. Under Option 1 (selected 2026-05-07), M4 is solo in W3 and M5+M6 are paired in W4. Pointing to M5 is accurate and sufficient; students will see the W4 pairing in the course calendar.

**Section C (cross-module) deferral.** Per the rubric, Section C runs after all 12 modules pass A and B individually. This scorecard reports A and B only.

**Branch state.** `polish/module-04` contains two commits ahead of main:
1. `polish(module-04): mechanical pass (format compliance)` — all Section A checks verified; B2 deepfakes paragraph and new orchestrator-verifier subsection included in this commit (consistent with M1 precedent)
2. `polish(module-04): judgment pass (AI-2026 currency, voice, CLO alignment)` — Discussion Prompt updated with DSA context; all Section B checks PASS on first pass
3. `polish(module-04): final scorecard, all rubric checks pass` — this file
