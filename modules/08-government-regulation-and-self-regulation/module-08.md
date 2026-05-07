# Module 8: Government Regulation and Self-Regulation

In January 2023, the Irish Data Protection Commission fined Meta Platforms a combined 390 million euros for violations of the European Union's General Data Protection Regulation (GDPR). The core issue was deceptively simple: Meta had been requiring users to agree to personalized advertising as a condition of using its services, treating consent as a checkbox buried in terms of service rather than a genuine, informed choice. European regulators concluded that this approach violated GDPR's requirement for freely given consent. For a company that generates the vast majority of its revenue from targeted advertising, the ruling struck at the heart of its business model. The fine was substantial, but the real impact was the message it sent: governments can and will hold technology companies accountable for how they handle personal data, even when those companies operate across international borders.

That case captures the central tension of this module. Technology companies operate at global scale and at speeds that outpace legislation. Governments attempt to protect citizens through regulation, but regulations vary across jurisdictions, sometimes conflict, and take years to draft and enforce. Meanwhile, professional organizations argue that self-regulation is faster, more flexible, and more technically informed than government mandates. The question you will examine is not whether regulation is necessary, but rather: who should set the rules for IT, how should those rules be enforced, and what happens when the people making the rules do not fully understand the technology they are regulating?

This module also addresses two workforce ethics topics that intersect with regulation: the H-1B visa program and offshore outsourcing, both of which involve government policy, corporate decision-making, and real consequences for workers in the United States and abroad.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + activities + discussion)
* **Prerequisites:** Modules 1-7
* **Deliverables:** Discussion post, Quick Checks, Skills Lab analysis
* **CLOs addressed:** CLO X

### Module Learning Objectives *(MLO)* 🎯

By the end of this module, **you will be able to**:

* MLO-8.1 (Apply): **Apply knowledge of key IT regulations (GDPR, CCPA, COPPA, HIPAA) to determine which laws govern specific data handling scenarios and identify compliance obligations** *(CLO X)*
* MLO-8.2 (Analyze): **Analyze the strengths and limitations of government regulation versus professional self-regulation in promoting ethical IT practices** *(CLO X)*
* MLO-8.3 (Evaluate): **Evaluate the ethical implications of IT workforce policies, including H-1B visa programs and offshore outsourcing, from multiple stakeholder perspectives** *(CLO X)*

---

## 8.1 Key IT Regulations and Their Scope

Repeated data breaches and unauthorized data sharing have demonstrated that trust alone is insufficient to protect personal data. Government regulations establish a baseline that all organizations must meet regardless of whether they would choose to do so voluntarily. If you work in IT, the decisions you make about data collection, storage, access, and sharing are governed by these laws, and the people whose data you handle are counting on you to get it right.

### The General Data Protection Regulation (GDPR)

The **General Data Protection Regulation (GDPR)**, enacted by the European Union in 2018, is widely regarded as the most comprehensive data privacy law in the world. It applies to any organization that processes the personal data of individuals located in the EU, regardless of where the organization itself is based. A company headquartered in Phoenix, Arizona, must comply with GDPR if it collects data from users in France or Germany.

GDPR is built on several core principles:

* **Lawful basis for processing:** Organizations must have a legitimate reason for collecting and using personal data. Consent must be freely given, specific, informed, and unambiguous; pre-checked boxes and bundled consent do not qualify.
* **Data minimization:** Collect only the data actually needed for the stated purpose.
* **Right of access and right to erasure:** Individuals can request a copy of their data and request deletion (the "right to be forgotten").
* **Data breach notification:** Notify the relevant supervisory authority within 72 hours of becoming aware of a breach that poses a risk to individuals' rights.
* **Penalties:** Fines up to 20 million euros or 4% of annual global revenue, whichever is higher. Meta, Amazon, and Google have all faced fines exceeding 100 million euros.

GDPR's extraterritorial reach means that companies worldwide have had to adjust their data practices, and its framework has inspired similar legislation in dozens of countries.

### The California Consumer Privacy Act (CCPA) and CPRA

The **California Consumer Privacy Act (CCPA)**, effective since January 2020, was the first comprehensive state-level data privacy law in the United States, later amended and expanded by the **California Privacy Rights Act (CPRA)** in 2023. Together, these laws give California residents significant rights over their personal data:

* **Right to know:** Consumers can request what personal information a business has collected, the sources, and who it has been shared with.
* **Right to delete:** Consumers can request deletion of their personal information, with some exceptions.
* **Right to opt out of sale:** Consumers can direct a business not to sell or share their personal information. The "Do Not Sell My Personal Information" link you see on many websites exists because of this requirement.
* **Non-discrimination:** Businesses cannot discriminate against consumers who exercise their privacy rights.

The CCPA/CPRA applies to for-profit businesses meeting certain thresholds: annual gross revenue above $25 million, processing data of 100,000 or more consumers, or deriving 50% or more of revenue from selling personal information. While a state law, its impact is national because many companies apply CCPA-level protections to all US users rather than maintaining separate California-specific systems.

### The Children's Online Privacy Protection Act (COPPA)

The **Children's Online Privacy Protection Act (COPPA)**, a federal law first enacted in 1998, specifically protects the online privacy of children under 13. Websites and online services directed at children, or that knowingly collect data from children, must:

* Provide clear and comprehensive privacy policies
* Obtain **verifiable parental consent** before collecting personal information from children
* Give parents the ability to review, delete, and control their child's data
* Not condition a child's participation on the collection of more data than is reasonably necessary

The Federal Trade Commission enforces COPPA and brought a $170 million fine against YouTube in 2019 for collecting children's personal data without parental consent.

### HIPAA: A Brief Recap

You studied **HIPAA** in depth in Module 6. It is relevant here as an example of sector-specific regulation: rather than broad cross-industry rules, HIPAA creates specific requirements for covered healthcare entities and their business associates, with penalties up to $1.5 million per violation category annually.

### The Regulatory Patchwork Problem

One of the biggest challenges facing IT professionals is that there is no single, unified federal data privacy law in the United States. Instead, you must comply with a patchwork of federal laws (COPPA, HIPAA, FERPA, GLBA), state laws (CCPA/CPRA in California, plus similar laws in Virginia, Colorado, Connecticut, and a growing number of others), and international regulations (GDPR). Each law has different definitions, different thresholds, different rights, and different enforcement mechanisms.

A healthcare company that operates a website accessible in the EU, collects data from California residents, and serves patients under 13 may simultaneously need to comply with HIPAA, GDPR, CCPA, and COPPA. Smaller organizations face a disproportionate burden; large corporations can afford dedicated compliance teams.

### Think About It 8.1 🧠

> You run a small online tutoring business based in Arizona. Most of your students are in the US, but a few are in Europe, and some are under 13. Which regulations might apply to your business? Do you think it is fair that a small business faces the same regulatory complexity as a multinational corporation? What would a more equitable regulatory system look like?

### Quick Check 8.1 ✅

1. Explain the difference between GDPR's approach to data privacy (comprehensive, applying to all sectors) and HIPAA's approach (sector-specific, applying only to healthcare). What are the advantages and disadvantages of each approach? *(Analyze)*

2. A mobile app company based in Texas discovers that its fitness tracking app has been collecting location data from users in Germany without explicit consent. Which regulation applies, and what are the company's obligations? *(Apply)*

3. Under COPPA, why is verifiable parental consent required before collecting data from children under 13? What ethical principle does this requirement reflect? *(Understand)*

---

## 8.2 Professional Self-Regulation and Social Audits

Government regulation is one approach to ensuring ethical behavior in IT. Another is **self-regulation**, where industries, professional organizations, and individual companies establish and enforce their own standards. The core question is whether organizations and professions can be trusted to police themselves effectively, or whether external oversight is necessary.

### How IT Professions Police Themselves

Unlike medicine and law, most IT roles have no mandatory government licensing requirement. The IT profession relies on voluntary certifications, professional association membership, and employer-enforced standards.

**Professional associations** such as the ACM, IEEE, and ISC2 maintain codes of ethics. Members who violate these codes can face sanctions from reprimand to expulsion. Since membership is voluntary, enforcement power is limited: a developer expelled from the ACM can continue working as a developer, unlike a physician who loses their medical license.

**Voluntary certifications** such as CompTIA Security+, CISSP, and PMP establish competency standards and often include ethics requirements. Losing a certification does not legally prevent work in IT, but can significantly affect career prospects for credential-dependent roles.

**Industry self-regulatory bodies** also play a role. The Payment Card Industry Security Standards Council maintains the **Payment Card Industry Data Security Standard (PCI DSS)** for any organization that processes credit card data. PCI DSS is technically a private standard but functions like regulation: organizations that fail to comply can lose the ability to process credit card payments.

### The Case For and Against Self-Regulation

Supporters argue that industry professionals understand their own technologies far better than legislators; that self-regulatory standards can be updated quickly while government regulations take years to draft and implement; and that heavy-handed regulation can stifle innovation by imposing compliance costs that discourage new market entry.

Critics counter that asking an industry to regulate itself creates a conflict of interest, since organizations have a financial incentive to set standards that are easy to meet rather than standards that genuinely protect the public. Self-regulatory bodies often lack authority to impose meaningful penalties, and self-regulation only works if all significant players participate. Companies that opt out gain a competitive advantage by cutting ethical corners while competitors bear compliance costs.

### Corporate and Professional Social Audits

A **social audit** is a formal assessment of an organization's social, ethical, and environmental performance. In IT, social audits examine data handling practices, algorithmic fairness, supply chain ethics, and diversity and inclusion. Third-party audits carry more credibility than internal ones, but even third-party audits have limits: scope is typically defined by the organization being audited, and organizations can choose not to publish unfavorable results.

### Case Study 8.1 - TechBridge and the Privacy Self-Assessment 📋

**The Situation:** TechBridge Analytics is a mid-size data analytics company that provides customer behavior tracking services to online retailers. TechBridge collects browsing data, purchase history, and location information from millions of consumers through tracking pixels and cookies embedded in its clients' websites.

In 2024, the Digital Advertising Alliance (DAA), an industry self-regulatory group, asks TechBridge to participate in a voluntary privacy compliance assessment. TechBridge's Chief Privacy Officer, Marcus Webb, agrees and assembles an internal team to conduct the review. The team discovers several concerning findings: TechBridge's data retention policies allow consumer data to be stored for seven years, far longer than necessary for the stated analytics purpose. Consumer opt-out requests are processed inconsistently, with some requests taking up to 90 days. Most significantly, TechBridge has been combining data sets from different clients to build comprehensive consumer profiles, a practice not disclosed in its privacy policy.

Marcus presents two options to the CEO, Diana Reeves. Option A: voluntarily disclose all findings to the DAA, update the privacy policy, reduce data retention to 18 months, and fix the opt-out process. This would cost approximately $2 million in system changes and could trigger client concern. Option B: report only the opt-out processing delay to the DAA (which is the easiest to fix), address data retention quietly over the next year, and continue the data combination practice after adding a vague disclosure to the privacy policy. Diana leans toward Option B, arguing that full disclosure would create competitive disadvantage and that the DAA has no real enforcement power anyway.

**Stakeholders:**

* **Consumers:** Millions of individuals whose browsing behavior, purchase history, and location data are being collected, stored, and combined without full knowledge or effective opt-out mechanisms
* **Marcus Webb (Chief Privacy Officer):** Responsible for privacy compliance. Discovered the problems through the audit and must decide how far to push back on the CEO's preferred approach
* **Diana Reeves (CEO):** Focused on competitive position and profitability. Views the DAA assessment as a public relations exercise rather than a meaningful accountability mechanism
* **TechBridge's retail clients:** Companies that embed TechBridge's tracking on their websites. They may not know that TechBridge is combining data across clients, which could expose them to legal liability
* **The Digital Advertising Alliance (DAA):** An industry self-regulatory body attempting to demonstrate that the advertising industry can regulate itself and does not need additional government oversight

**Questions to Consider:**

1. Does the DAA's lack of enforcement power change TechBridge's ethical obligations? If self-regulation has no real consequences for non-compliance, what purpose does it serve?
2. Marcus discovered the problems through an internal audit. If Diana proceeds with Option B (partial disclosure), does Marcus have an obligation to report to an external authority? Consider the whistleblowing frameworks from Module 5.
3. If you were a consumer whose data was being handled this way, would you prefer that a government regulator like the FTC enforced strict privacy rules, or that the industry self-regulated through organizations like the DAA? What does your preference reveal about the strengths and weaknesses of self-regulation?

### Think About It 8.2 🧠

> Many social media companies have established internal "trust and safety" teams to moderate content and enforce community standards. This is a form of self-regulation. In your experience as a social media user, do you believe these teams are effective at protecting users from harmful content? What incentives might lead a company's self-regulation to fall short?

### Quick Check 8.2 ✅

1. Explain why IT professionals are generally not required to hold a government-issued license, unlike doctors or lawyers. What are the consequences of this difference for professional accountability? *(Understand)*

2. A cybersecurity company voluntarily follows the NIST Cybersecurity Framework but is not legally required to do so. If the company suffers a data breach despite following the framework, should the company receive legal credit for following voluntary standards? Analyze the ethical argument for and against this position. *(Analyze)*

3. A professional association revokes an IT consultant's certification for violating the organization's code of ethics. The consultant continues working in IT at the same level because the certification was not required for their role. Evaluate whether this outcome suggests that professional self-regulation is effective or ineffective. *(Evaluate)*

---

## 8.3 IT Workforce Ethics: H-1B Visas and Offshore Outsourcing

The ethical dimensions of IT extend beyond data and software to include the people who build and maintain technology systems. Two workforce issues sit at the intersection of government regulation, corporate strategy, and ethical obligation: the H-1B visa program and offshore outsourcing.

### The H-1B Visa Program

The **H-1B visa** allows US employers to temporarily hire foreign workers in specialty occupations requiring at least a bachelor's degree. The technology industry is the largest user of H-1B visas.

The program operates on several key mechanisms:

* **Annual cap:** Currently 65,000 new visas annually (plus 20,000 for workers with US advanced degrees). Because demand far exceeds supply, visas are allocated by lottery.
* **Employer sponsorship:** The visa is tied to a specific employer. Changing jobs requires transferring the visa, which creates a dependency relationship.
* **Prevailing wage requirement:** Employers must pay H-1B workers at least the **prevailing wage** for the position in that geographic area.

### Ethical Concerns with the H-1B Program

**The talent argument:** Technology companies argue the H-1B program is essential for filling genuine skill gaps. When there are not enough qualified US workers for highly specialized roles, H-1B visas allow companies to recruit the best talent globally. Supporters point to the many H-1B holders who have made transformative contributions to American technology and who have gone on to found startups and create jobs.

**The displacement concern:** Critics argue that some companies use the H-1B program not to fill genuine skill gaps but to replace existing US workers with lower-paid foreign workers. In 2015, Southern California Edison laid off approximately 400 IT workers and replaced many of them with H-1B visa holders employed through outsourcing firms. Workers were required to train their H-1B replacements as a condition of receiving severance packages.

**The power imbalance:** Because H-1B visas are tied to a specific employer, workers pursuing permanent residency through their employer face significant pressure. For workers from countries with high demand, the green card queue can mean a wait of 10 to 20 years. This dependency can make H-1B workers reluctant to report workplace problems, negotiate for higher pay, or push back against unethical practices.

**The outsourcing firm model:** A substantial portion of H-1B visas goes to IT outsourcing firms that contract workers to other companies. Critics argue this model turns the H-1B program into a labor arbitrage mechanism. Supporters counter that outsourcing firms provide legitimate staffing flexibility and that the prevailing wage requirement prevents underpayment.

### Offshore Outsourcing Ethics

**Offshore outsourcing** (or **offshoring**) is the practice of contracting work to companies or workers in other countries, typically to reduce costs. Common offshored IT functions include software development, customer support, data entry, quality assurance testing, and infrastructure management.

Arguments for offshoring include lower labor costs that allow companies to do more with the same budget, more affordable technology products for consumers, well-paying jobs relative to local economies in developing countries, and "follow the sun" development through time zone differences.

Ethical concerns include domestic job displacement (when a company moves 500 IT jobs from Ohio to India, 500 workers lose their livelihoods), potentially poor working conditions abroad, data security risks when sensitive data is processed under different legal protections, and the hollowing out of local economies that depend on technology employment.

### The Ethical Middle Ground

An ethically responsible approach includes using H-1B visas only where qualified domestic candidates are genuinely unavailable; paying H-1B workers at genuine market rates with equivalent working conditions; investing in retraining and severance when offshoring displaces domestic workers; and being transparent with employees and the public about the reasons and trade-offs.

### Quick Check 8.3 ✅

1. Explain the "power imbalance" concern with H-1B visas. Why does tying a visa to a specific employer create ethical risks for workers? *(Understand)*

2. A company offshores its customer support center to save $4 million annually. Sixty workers in the US lose their jobs. The company offers each displaced worker two weeks of severance and no retraining assistance. Apply the stakeholder analysis framework from Module 3 to evaluate whether the company's approach is ethically adequate. *(Apply)*

3. Some argue that H-1B visa reform should make it easier for workers to change employers without losing their immigration status. Others argue this would increase job competition for US workers. Analyze this trade-off from both a utilitarian and a deontological perspective. *(Analyze)*

---

## 8.4 Balancing Regulation with Innovation and Emerging AI Regulation

Every regulation creates compliance costs that are not spent on innovation. Every absence of regulation creates opportunities for exploitation and harm. The tension between regulation and innovation is not a problem to be solved once; it is a balancing act that must be continuously reassessed as technology evolves.

### The Regulatory Spectrum

The **precautionary approach** holds that new technologies should be restricted until they are proven safe, prioritizing harm prevention over innovation speed. The advantage is protection before harm occurs; the disadvantage is potentially delaying beneficial innovations and placing the burden of proof on innovators.

The **permissive approach** holds that innovation should proceed with minimal restriction, with regulation introduced only after specific harms are identified. The US approach to internet regulation in the 1990s and 2000s reflected this philosophy. The advantage is rapid development; the disadvantage is that harms may occur before rules exist, and once an industry is established, regulating it becomes politically and practically more difficult.

### AI Touchpoint: Emerging AI Regulation

The rapid deployment of AI systems has triggered what may be the most significant regulatory debate in the history of technology. Module 3 introduced the EU AI Act and NIST AI RMF frameworks. Module 8 extends those foundations with the regulatory specifics that matter most to your work as an IT professional in 2025-2026.

**The EU AI Act** entered into force in August 2024 and began phasing in obligations through 2025 and 2026. It takes a **risk-tiered approach**, classifying AI systems by the level of risk they pose:

* **Unacceptable risk:** Banned outright. This includes government social scoring, real-time remote biometric identification in public spaces (with limited law enforcement exceptions), and AI systems that manipulate human behavior to cause harm.
* **High risk:** Permitted but strictly regulated. AI systems used in employment decisions, credit scoring, law enforcement, education, and healthcare must complete mandatory conformity assessments, maintain detailed technical documentation, register in the EU AI database, and provide users with meaningful human oversight mechanisms. **High-risk obligations began phasing in during August 2025.** Organizations deploying AI hiring tools, credit-scoring algorithms, or healthcare diagnostic systems in EU markets must now either demonstrate compliance or cease operation.
* **Limited risk:** Transparency obligations apply. Chatbots must inform users they are interacting with AI; deepfake content must be labeled as artificially generated.
* **Minimal risk:** Spam filters, AI-enabled games, and similar low-risk systems face no additional regulatory requirements beyond existing laws.

For IT professionals in organizations that sell into EU markets or process EU resident data, the high-risk tier is the most consequential. Deploying an AI-powered hiring platform, loan underwriting tool, or clinical decision support system without completing the required conformity assessment is now a compliance violation, not just an ethical concern.

**US Federal AI Regulation in 2025-2026**

The United States continues a more permissive, sector-specific approach. In January 2025, the incoming administration rescinded Executive Order 14110 (Biden's 2023 AI safety order), signaling a lighter federal regulatory posture. The primary US regulatory action now flows through agencies:

* **FTC:** Using existing authority over unfair and deceptive practices to pursue companies that make false claims about AI accuracy or fairness, or that use AI in ways that harm consumers.
* **EEOC:** 2024-2025 guidance confirms that existing anti-discrimination law applies fully to AI-powered hiring tools. Employers who rely on automated screening without human review of disparate-impact outcomes face Title VII exposure.
* **CISA and OMB:** 2025 guidance requires federal agencies deploying AI to complete risk assessments aligned with the NIST AI RMF, requirements that extend to government contractors.
* **State-level action:** Colorado's AI Act (effective February 2026) requires reasonable care to protect consumers from algorithmic discrimination and annual impact assessments for high-risk AI. Texas, Virginia, and others have similar legislation advancing.

**Your Role as Orchestrator-Verifier**

Module 3 established the orchestrator-verifier frame: you direct AI systems and bear responsibility for verifying their outputs. Module 8's regulatory landscape gives that frame a compliance dimension. When you deploy or configure an AI system in an organizational context, you must determine which regulatory tier applies, verify that the system's documentation and human oversight mechanisms meet those requirements, and escalate gaps before deployment rather than after a regulator identifies them. Accepting vendor assurances of "compliance" without reviewing underlying documentation is not adequate due diligence. The regulatory expectation in 2025-2026 is that the organization deploying the AI bears primary accountability.

**The NIST AI Risk Management Framework (AI RMF)**

The **NIST AI RMF** (released January 2023) is a voluntary framework organized around four core functions: **Govern** (establish policies for managing AI risks), **Map** (understand the context and identify potential risks), **Measure** (assess risks quantitatively and qualitatively), and **Manage** (prioritize and act on risks based on impact). Courts and regulators cite it as a benchmark for "reasonable care" in AI deployment, and under 2025 OMB guidance, federal contractors are now effectively required to align with it.

### Think About It 8.4 🧠

> The EU AI Act bans social scoring (government systems that rate citizens based on their behavior and assign consequences). China has implemented systems that some observers describe as social scoring. The US has not banned the practice but has not implemented it either. Where do you think the line should be drawn between using data to improve public safety and using data to control citizens? Who should decide where that line falls?

### Quick Check 8.4 ✅

1. Describe the four risk tiers of the EU AI Act and give one example of an AI application that would fall into each tier. *(Understand)*

2. A US company develops an AI system that screens job applicants by analyzing their facial expressions during video interviews. The company plans to sell this system to employers in both the US and the EU. Analyze how the regulatory requirements would differ in each jurisdiction and identify which approach better protects job applicants from potential bias. *(Analyze)*

3. Some critics argue that the NIST AI RMF is ineffective because it is voluntary, while supporters argue that voluntary frameworks are more practical and adaptable than laws. Evaluate both positions. Under what circumstances would a voluntary framework be sufficient, and when is binding regulation necessary? *(Evaluate)*

---

## 8.5 Skills Lab 8A - Regulatory Analysis of an AI Hiring Platform

**Goal:** Analyze a realistic scenario involving an AI-powered hiring platform to evaluate how government regulations, self-regulatory standards, and workforce ethics principles intersect in a single business decision.

**Estimated time:** 90-120 minutes

### Scenario: HireRight AI Expands Internationally

HireRight AI is a Phoenix-based startup that has developed an AI-powered hiring platform called TalentScreen. The platform uses natural language processing to analyze resumes, machine learning to rank candidates, and video analysis to evaluate communication skills during recorded interviews. TalentScreen has been used by over 200 US companies since its launch in 2023 and has processed more than 2 million job applications.

HireRight AI is preparing to expand into Europe, with initial clients lined up in Germany and France. Simultaneously, the company is facing scrutiny at home. A civil rights organization has published a report alleging that TalentScreen systematically ranks candidates from historically Black colleges and universities (HBCUs) lower than candidates from predominantly white institutions, even when candidates have comparable qualifications. HireRight AI disputes the findings but has not published its own analysis.

The company's expansion plan also involves significant workforce changes. HireRight AI plans to offshore its data annotation team (currently 45 workers at its Phoenix office) to a contractor in the Philippines to reduce annotation costs by 60%. The annotation team was told about the plan two weeks ago and given 90 days' notice. No retraining or transition assistance has been offered. Additionally, HireRight AI sponsors 12 software engineers on H-1B visas, and two of those engineers have privately expressed concerns about the algorithmic bias allegations but are reluctant to raise them formally because their green card applications are pending.

The company's CEO, Raj Anand, has asked his leadership team to prepare a compliance and ethics review before the European launch. He wants to ensure the company meets regulatory requirements but also wants to move quickly because two competitors are also expanding into Europe.

### Part 1: Foundation (Aligns with LO1)

1. Identify which specific regulations (from Section 8.1) apply to HireRight AI's operations. Consider both its current US operations and its planned European expansion. For each regulation, explain what specific compliance obligations HireRight AI must meet.

2. The EU AI Act classifies AI systems by risk level. At which risk tier would TalentScreen most likely be classified under the EU AI Act? Explain your reasoning, referencing the specific characteristics of TalentScreen and the risk tier definitions from Section 8.4.

3. The NIST AI RMF is a voluntary framework. If HireRight AI adopted it, which of the four core functions (Govern, Map, Measure, Manage) would be most immediately relevant to addressing the algorithmic bias allegation? Explain how that function would apply.

### Part 2: Application (Aligns with LO2)

4. Analyze whether industry self-regulation would be sufficient to address the algorithmic bias allegations against TalentScreen, or whether government regulation is necessary. Reference the arguments for and against self-regulation from Section 8.2.

5. Evaluate HireRight AI's handling of the offshoring decision. Using the ethical principles from Section 8.3, identify at least three specific ways the company could make this transition more ethically responsible.

6. Consider the situation of the two H-1B engineers who have concerns about algorithmic bias but are reluctant to speak up. Analyze how the H-1B visa structure contributes to this silence and explain why this is an ethical problem for HireRight AI, not just a personal problem for the engineers.

### Part 3: Extension (Aligns with LO3)

7. Write a 200-word memo to CEO Raj Anand recommending whether HireRight AI should adopt a precautionary or permissive approach to its European launch. Your memo should reference at least two specific regulatory requirements and explain the ethical trade-offs of moving quickly versus moving carefully.

8. Evaluate the following claim: "If HireRight AI meets all legal compliance requirements in both the US and EU, it has fulfilled its ethical obligations." Do you agree or disagree? Support your position with at least one ethical framework from Module 1 and specific examples from the scenario.

### Rubric

| Criteria | Mastery (5) | Proficiency (4) | Developing (3) | Emerging (2) | Not Evident (1) |
|---|---|---|---|---|---|
| **Stakeholder Analysis** | Identifies all major stakeholders with specific, accurate descriptions of their interests and what each stands to gain or lose | Identifies most stakeholders with reasonable descriptions of their interests | Identifies some stakeholders but descriptions lack specificity or miss key interests | Lists stakeholders without meaningful description of their interests | Missing or inaccurate |
| **Ethical Framework Application** | Applies ethical frameworks accurately with clear reasoning and specific references to scenario details; demonstrates understanding of each framework's logic | Applies frameworks correctly with adequate reasoning and some scenario-specific references | Applies frameworks but with gaps in reasoning or limited connection to the scenario | Attempts to apply frameworks but with significant errors or confusion between them | Missing or not recognizable as framework application |
| **Module Concept Application** | Accurately applies module-specific concepts to the scenario with detailed, well-reasoned analysis that demonstrates mastery of the material | Applies module-specific concepts correctly with adequate reasoning and clear connections to the scenario | References module concepts but application is incomplete or partially inaccurate | Mentions module concepts without meaningful application to the scenario | No application of module concepts attempted |
| **Recommendation Quality** | Recommendation is clear, specific, and well-supported by multiple frameworks with explicit reasoning; addresses counterarguments or competing interests | Recommendation is clear and supported by at least one framework with reasonable justification | Recommendation is present but weakly supported or lacks clear connection to ethical reasoning | Recommendation is vague, generic, or unsupported by ethical reasoning | No recommendation provided |
| **Writing and Professionalism** | Writing is clear, well-organized, and uses ethical and professional terminology accurately throughout; ideas flow logically between sections | Writing is clear with mostly accurate terminology and reasonable organization | Writing is understandable but disorganized or imprecise in terminology use | Writing is unclear, contains frequent errors, or lacks professional tone | Unreadable or off-topic |

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.
* **Due:** See Canvas calendar for deadline

---

## 8.6 Summary and Retrieval 💡

### Key Concepts

* **Major IT regulations create enforceable data protection standards.** GDPR provides comprehensive, cross-sector privacy protection with significant extraterritorial reach. CCPA/CPRA gives California consumers specific data rights. COPPA protects children under 13. HIPAA addresses healthcare data. Together, these laws form a patchwork that IT professionals must understand and manage, often simultaneously.

* **Self-regulation and government regulation each have strengths and weaknesses.** Self-regulation is faster, more technically informed, and more flexible; government regulation is more enforceable and less susceptible to industry conflicts of interest. The most effective approach combines both: industry standards backed by government enforcement for organizations that fall short.

* **Social audits are only as strong as the commitment behind them.** Honest social audits can identify and correct ethical gaps. When audits are treated as public relations exercises with selective disclosure, they undermine the credibility of self-regulation entirely.

* **H-1B visa programs and offshore outsourcing raise genuine ethical tensions.** These workforce practices create real benefits and real harms. Ethical approaches require transparency, fair treatment of all workers, and meaningful transition support for displaced employees.

* **AI regulation is the defining regulatory challenge of our time.** The EU AI Act's high-risk obligations began phasing in during August 2025, making conformity assessments mandatory for AI systems in employment, credit, and healthcare. US regulation remains sector-specific and agency-driven; state laws including Colorado's AI Act add a growing layer of accountability. The NIST AI RMF is the voluntary benchmark regulators increasingly cite as the standard for reasonable care. As orchestrator-verifier, you are accountable for verifying that AI systems you deploy meet applicable requirements before deployment.

* **The tension between regulation and innovation is ongoing.** Over-regulation risks stifling beneficial development. Under-regulation risks allowing harm. IT professionals have both a compliance obligation and an ethical obligation to engage with these questions rather than treating regulation as merely a cost to be minimized.

### Key Terms

* **GDPR:** The EU's comprehensive data privacy law (2018) applying to any organization processing personal data of EU residents, regardless of where the organization is based
* **CCPA / CPRA:** California state laws giving consumers rights over their personal data, including the right to know, delete, and opt out of data sales
* **COPPA:** A US federal law requiring verifiable parental consent before collecting personal information from children under 13 online
* **Verifiable parental consent:** COPPA's requirement for provable parental or guardian permission before collecting a child's data
* **Self-regulation:** An industry or profession establishing and enforcing its own ethical standards without government mandate
* **Social audit:** A formal assessment of an organization's social, ethical, and environmental performance against its stated values
* **PCI DSS:** An industry-created security standard required for all organizations that process credit card data
* **H-1B visa:** A US work visa allowing employers to temporarily hire foreign workers in specialty occupations requiring at least a bachelor's degree
* **Prevailing wage:** The average wage for an occupation and geographic area that employers must meet or exceed when hiring H-1B workers
* **Offshore outsourcing (offshoring):** Contracting IT work to companies or workers in other countries, typically to reduce labor costs
* **Precautionary approach:** A regulatory philosophy that restricts new technologies until they are proven safe
* **Permissive approach:** A regulatory philosophy that allows innovation to proceed with minimal restriction, introducing regulation only after specific harms are identified
* **EU AI Act:** The world's first comprehensive AI regulation, risk-tiered; high-risk obligations began phasing in August 2025
* **NIST AI RMF:** A voluntary US framework (Govern, Map, Measure, Manage) for identifying, assessing, and mitigating AI risks throughout a system's lifecycle

### Retrieval Practice

Try to answer these from memory before looking back at the module.

1. Name and briefly describe four major IT regulations and identify the type of data or population each one protects. Then explain why the lack of a single unified federal privacy law in the US creates challenges for IT professionals.

2. What are the main arguments for and against professional self-regulation in IT? Give one real-world example of self-regulation working effectively and one example of it falling short.

3. Explain the difference between the EU's precautionary approach and the US's permissive approach to AI regulation. Which approach do you believe better balances innovation with public protection, and why?

---

## 8.7 Discussion Prompt 💬

**Prompt:** In 2015, Southern California Edison laid off approximately 400 IT workers and replaced many of them with H-1B visa holders employed through outsourcing firms. Several of the displaced workers reported that they were required to train their replacements as a condition of receiving severance pay. Supporters of the H-1B program argue that it fills genuine skill gaps and that companies must be able to access global talent to remain competitive. Critics argue that cases like this show the program is being used primarily as a cost-cutting tool at the expense of American workers.

To what extent should companies be free to make workforce decisions based on cost efficiency, and at what point do ethical obligations to existing workers override financial considerations? Take a clear position, support it with at least one concept from this module (regulatory frameworks, self-regulation principles, stakeholder analysis, or workforce ethics), and address the strongest counterargument to your position.

**Guidelines:**

* Your initial post should be 200-300 words
* Reference at least one ethical framework or concept from this module
* Respond to at least two classmates with substantive engagement

---

## Further Reading 📖

* **European Commission: "The EU AI Act."** Full text and explanatory materials for the world's first comprehensive AI regulation, including risk tier definitions and phase-in timelines. Free at digital-strategy.ec.europa.eu.

* **NIST: "AI Risk Management Framework (AI RMF 1.0)."** The complete voluntary framework for managing AI risks, including the Govern, Map, Measure, and Manage functions. Free at nist.gov.

* **California Office of the Attorney General: "California Consumer Privacy Act (CCPA)."** Official guidance on CCPA and CPRA compliance, consumer rights, and enforcement. Free at oag.ca.gov.

* **Federal Trade Commission: "Protecting Kids' Privacy."** FTC guidance on COPPA compliance and enforcement actions. Free at ftc.gov.

* **Hira, Ron. "The H-1B and L-1 Visa Programs: Out of Control."** An Economic Policy Institute briefing paper examining the use of temporary work visa programs in the technology industry. Free at epi.org.

---

## Looking Ahead ⏩

In Module 9, you will shift from the rules that govern organizations and workers to the rules that govern ideas and creative works. You will examine the four main types of intellectual property (copyright, patents, trademarks, and trade secrets), explore the fair use doctrine and its limits in digital contexts, and consider the ethics of open source licensing, plagiarism, reverse engineering, and digital piracy. You will also confront one of the most contested legal questions in technology today: who owns content created by an AI, and did AI companies violate copyright law by training their models on data scraped from the internet? Under the selected course schedule, Module 9 is paired with Module 10 in Week 7 (July 6-12), so the two modules together form a focused week on rights in digital contexts.
