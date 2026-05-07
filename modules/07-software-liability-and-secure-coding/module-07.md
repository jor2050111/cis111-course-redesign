# Module 7: Software Liability and Secure Coding

On July 19, 2024, a routine software update from cybersecurity firm CrowdStrike caused approximately 8.5 million Windows computers to crash simultaneously. Airlines grounded flights. Hospitals postponed surgeries. Banks froze transactions. Emergency 911 systems went offline in several states. The cause was not a cyberattack. It was a single flawed configuration file pushed through an automated update process that had insufficient testing safeguards. One software defect, distributed at scale, disrupted critical systems worldwide in a matter of hours.

This incident is not an outlier. Software failures have caused passenger jets to crash, medical devices to deliver lethal radiation doses, and the personal data of hundreds of millions of people to be exposed. As software becomes embedded in everything from pacemakers to power grids, the question of who is responsible when that software fails is no longer theoretical. It is urgent, and it directly affects you as an IT professional.

This module examines software liability, software quality, secure coding practices, and the ethical dimensions of cost/benefit analysis in IT decision-making. You will explore how product liability law applies (and sometimes fails to apply) to software, why development methodologies carry ethical weight, and what happens when organizations cut corners on security to save time or money. You will also examine a question that is rapidly becoming one of the most important in technology: when an AI system causes harm, who should be held accountable?

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + activities + discussion)
* **Prerequisites:** Modules 1-6
* **Deliverables:** Discussion post, Quick Checks, Skills Lab analysis
* **CLOs addressed:** CLO VIII, CLO IX

### Module Learning Objectives *(MLO)* 🎯

By the end of this module, **you will be able to**:

* MLO-7.1 (Apply): **Apply product liability concepts, including negligence, strict liability, and warranty frameworks, to real-world software failure scenarios** *(CLO VIII)*
* MLO-7.2 (Analyze): **Analyze the ethical obligations of software developers and organizations regarding software quality, secure coding, and vulnerability management** *(CLO VIII)*
* MLO-7.3 (Evaluate): **Evaluate cost/benefit trade-offs in IT decision-making, particularly in safety-critical systems and AI deployment** *(CLO IX)*

---

## 7.1 Software Defects and Product Liability

A **software defect** (commonly called a "bug") is an error or unintended behavior in a program that causes incorrect or unexpected results. Some defects are trivial: a button displaying the wrong color, or a date that formats incorrectly. Others are deadly. In the late 1980s, the Therac-25 radiation therapy machine delivered massive radiation overdoses to at least six patients due to a software race condition. Three died. The software had been reused from an earlier model without adequate testing for the new hardware.

The critical ethical question is not whether defects will occur (they will), but what obligations developers and organizations have to prevent, detect, and respond to them.

### Product Liability Frameworks

When a physical product injures someone, **product liability** law provides a framework for holding the manufacturer responsible. Software complicates that framework in several ways. Three theories cover most claims:

* **Negligence** requires proving that the developer or company failed to exercise reasonable care: ignoring known defects, skipping industry-standard testing, or rushing a release without adequate quality assurance. If a company knew about a critical vulnerability but shipped the product anyway to meet a deadline, a negligence claim has strong footing.

* **Strict liability** holds manufacturers responsible for defective products regardless of how careful they were. The question is not "Did you try hard enough?" but "Was the product defective, and did it cause harm?" Courts have been reluctant to apply strict liability uniformly to software.

* **Breach of warranty** occurs when software fails to perform as promised. Warranties can be **express** (explicitly stated in marketing or contracts) or **implied** (assumed by law, such as the implied warranty that a product is fit for its intended purpose).

### Is Software a "Product" or a "Service"?

This is one of the most contested questions in software liability law. When you purchase software on a disc or embedded in a device, courts are more likely to treat it as a product subject to product liability. When you access software through a cloud service or subscription (Software as a Service, or **SaaS**), courts have sometimes classified it as a service, which carries weaker liability standards. This distinction matters: if software is a product, strict liability may apply; if it is a service, the injured party must prove negligence, a higher burden.

The trend toward SaaS delivery means that much of the software you interact with daily exists in a legal gray area, and vendors may argue that product liability does not apply.

### Liability Limitations: EULAs and Terms of Service

Before you can use most software, you must agree to an **End User License Agreement (EULA)** or **Terms of Service (ToS)**. These agreements almost always limit the company's liability, with disclaimers like "the software is provided 'as is'" and caps on damages at the price you paid.

Most users never read EULAs. Even those who do often have no practical alternative: you agree or you cannot use the software. When a clause says a company bears no responsibility if its software exposes your data, is that a fair agreement or an exploitation of the power imbalance between a large company and an individual user?

Courts have sometimes found egregious limitations **unconscionable** and unenforceable. In practice, most hold up, giving software vendors a level of liability protection that manufacturers of physical products do not enjoy.

### Think About It 7.1 🧠

> You install a popular antivirus program that promises "comprehensive protection against all known threats." A new strain of ransomware encrypts your files, and the antivirus software fails to detect it. The EULA says the company is not liable for any damages. Do you think the company has an ethical obligation to compensate you, even if the EULA says otherwise? What if the same ransomware affected a hospital and disrupted patient care?

### Quick Check 7.1 ✅

1. Explain the difference between negligence and strict liability in product liability law. Why does it matter which standard applies to software? *(Understand)*

2. A cloud-based accounting service has a defect that causes a small business to lose three months of financial records. The company argues that because their product is a service (SaaS), not a product, strict liability should not apply. Using what you learned about the product-vs.-service distinction, explain whether this argument is ethically defensible, even if it is legally valid. *(Analyze)*

3. A software company discovers a known defect in their hospital patient management system but decides to delay the fix until the next scheduled update in three months. Identify which product liability theory (negligence, strict liability, or breach of warranty) best applies to this situation and explain why. *(Apply)*

---

## 7.2 Software Quality and Development Ethics

Software quality is not just a technical concern. It is an ethical one. When organizations choose how to build, test, and maintain their software, they are making decisions that affect everyone who depends on that software.

### What Does Software Quality Mean?

**Software quality** refers to the degree to which software meets its specified requirements and satisfies user needs. From an ethical standpoint, quality also means the software does not cause unnecessary harm, performs honestly, and communicates its limitations transparently.

Quality is not binary. A game with a minor graphical glitch has different quality obligations than a medical device that controls insulin dosing. Potential for harm shapes the ethical standard.

### The Capability Maturity Model Integration (CMMI)

The **Capability Maturity Model Integration (CMMI)** measures an organization's software development process maturity across five levels:

| Level | Name | Description |
|-------|------|-------------|
| 1 | Initial | Processes are unpredictable and reactive. Success depends on individual effort. |
| 2 | Managed | Projects are planned and tracked. Basic project management is in place. |
| 3 | Defined | Processes are standardized across the organization. Consistent practices exist. |
| 4 | Quantitatively Managed | Processes are measured and controlled using statistical data. |
| 5 | Optimizing | Organization focuses on continuous improvement based on data and innovation. |

Most organizations operate at Level 1 or 2. Higher levels produce more predictable, reliable software. Organizations that choose to remain at Level 1, accepting chaotic and unpredictable processes, are making a choice that affects everyone who depends on their software.

### Development Methodologies and Their Ethical Dimensions

How software is built shapes whether it is built well. Three dominant development methodologies each carry distinct ethical implications:

**Waterfall** is a sequential process: requirements, then design, then coding, then testing, then deployment. Its strength is thoroughness in planning and documentation. Its ethical risk is rigidity: if requirements change or new risks emerge during development, waterfall makes it difficult to adapt. Software built under waterfall may be well-documented but slow to respond to discovered vulnerabilities.

**Agile** is an iterative approach that delivers working software in short cycles (typically two-week "sprints"). Its ethical strength is adaptability: if a security flaw is discovered, agile teams can prioritize a fix in the next sprint. Its ethical risk is that pressure to ship quickly can lead teams to cut corners on testing, documentation, or security reviews. When a product owner says "ship it now, fix it later," ethical problems follow.

**DevOps** extends agile by integrating development and operations teams through automation, continuous integration, and continuous delivery (CI/CD). DevOps enables rapid deployment of patches, which is an ethical advantage. However, speed without adequate safety checks creates ethical liability. The 2024 CrowdStrike incident is a cautionary example: an automated deployment pipeline pushed a flawed update to millions of machines because the pipeline's testing safeguards were insufficient.

### Technical Debt and Ethical Implications

**Technical debt** is the accumulated cost of shortcuts taken during software development. When a team writes quick-and-dirty code to meet a deadline, they take on technical debt. The code works now but will be harder to maintain, harder to secure, and more likely to break in the future.

Technical debt is a business decision, but it is also an ethical one. When organizations knowingly accumulate technical debt without a plan to address it, they transfer risk from themselves to their users. Users bear the consequences of crashes, data loss, and security breaches, while the organization benefited from the faster delivery that created the debt.

### Case Study 7.1 - The MedTrack Patient Monitoring Dilemma 📋

**The Situation:** MedTrack Solutions is a mid-size software company that develops patient monitoring systems for regional hospitals. Their flagship product, VitalWatch, tracks patient heart rate, blood pressure, and oxygen levels in real time and alerts nursing staff when readings fall outside safe ranges.

During a routine code review, senior developer Priya Nair discovers a defect in VitalWatch's alert logic. Under specific conditions (when a patient's heart rate drops below 40 beats per minute while oxygen saturation simultaneously falls below 88%), the system fails to trigger an alert. Instead, it logs the readings as normal. Priya estimates the defect affects roughly 2% of critical care patients.

Priya reports the defect to her manager, David Chen. David acknowledges the severity but explains the situation: MedTrack is in the middle of a major sales push. They are competing for a contract with a hospital network that would double the company's revenue. David tells Priya that disclosing the defect now would derail the sales process and could lead to lawsuits from existing hospital clients. He asks her to document the bug internally and schedule the fix for the next quarterly release, three months away. He adds that the 2% occurrence rate is low and that nursing staff should catch most of those situations through manual monitoring anyway.

Priya is uncomfortable with this plan. She knows that in critical care, a missed alert could mean a patient dies. But she also knows that MedTrack employs 200 people, and losing the contract could lead to layoffs. She has a mortgage and a child in daycare.

**Stakeholders:**
* **Priya Nair (senior developer):** Discovered the defect. Feels a professional obligation to ensure patient safety but faces personal and professional risk if she escalates.
* **David Chen (engineering manager):** Responsible for the product timeline and aware of the company's financial pressures. Prioritizing the sales contract over an immediate fix.
* **Hospital clients and patients:** Currently using a product with a known defect that could fail to alert staff during a life-threatening event. They do not know about the defect.
* **MedTrack Solutions (company):** Faces financial risk from disclosure and legal risk from non-disclosure. Two hundred employees depend on the company's stability.
* **Nursing staff:** Responsible for patient care. May rely on VitalWatch alerts as a safety net and may not catch every critical event through manual checks alone.

**Questions to Consider:**
1. Using the product liability frameworks from Section 7.1, which theory of liability (negligence, strict liability, or breach of warranty) would most likely apply if a patient is harmed because of this defect? Explain your reasoning.
2. Consider David's argument that the 2% occurrence rate is low and that nurses provide a backup. Is this an acceptable risk assessment, or is it a rationalization? How does the severity of potential harm change the calculation?
3. If you were Priya, what would you do? Identify which ethical framework (from Module 1) supports your decision and explain how you weighed the competing interests of patient safety, job security, and company viability.

### Quick Check 7.2 ✅

1. Name and briefly describe the five CMMI maturity levels. At which level would you expect the most reliable and predictable software development outcomes? *(Remember)*

2. A startup uses agile development and ships a new feature every two weeks. They have no dedicated security review process because it would slow their release cycle. Analyze the ethical trade-off the startup is making and identify who bears the risk. *(Analyze)*

3. Explain the concept of technical debt using a non-technical analogy. Then describe one way that technical debt creates ethical risk for software users. *(Understand)*

---

## 7.3 Secure Coding and Vulnerability Management

Secure coding is not an optional enhancement or an afterthought added before release. It is a fundamental ethical obligation for anyone who writes, reviews, or deploys software. When developers fail to follow secure coding practices, they create vulnerabilities that expose users to data theft, financial loss, and even physical danger.

### What Is Secure Coding?

**Secure coding** is the practice of writing software that protects against security vulnerabilities by design. The core principle: every input is potentially malicious, every connection is potentially hostile, and every assumption about how the software will be used is potentially wrong. These are design constraints from the start, not afterthoughts.

The **Open Web Application Security Project (OWASP)** maintains the OWASP Top 10, a regularly updated list of the most critical web application security risks.

### Common Vulnerability Types

As an IT professional, knowing the basic vulnerability categories helps you understand security risks, evaluate vendor claims, and participate in security discussions. You do not need to be a programmer.

**Injection flaws** occur when an attacker sends malicious data that a program treats as a command. The most common type is **SQL injection**: an attacker enters specially crafted text into a web form, and the application passes it directly to a database query. Without proper input validation, the attacker can read, modify, or delete database contents.

**Authentication and session management flaws** involve weaknesses in how software verifies identity: storing passwords in plain text, allowing weak passwords, failing to expire session tokens, or skipping multi-factor authentication for sensitive operations.

**Cross-site scripting (XSS)** occurs when an application includes untrusted data in a web page without validation, allowing attackers to inject malicious scripts that execute in other users' browsers. XSS is particularly dangerous because the malicious code runs in the context of a trusted website.

**Insecure direct object references** occur when an application exposes internal details (database record numbers, file paths) in URLs without checking authorization. A medical records portal where changing the patient ID in the URL reveals a different patient's records is a classic example.

**Security misconfiguration** refers to systems deployed with default settings, unnecessary features enabled, or incomplete configurations. It is one of the most common vulnerabilities because it results not from a coding error but from failure in deployment and maintenance.

### Responsible Disclosure vs. Full Disclosure

When a security researcher discovers a vulnerability in someone else's software, they face an ethical choice about how to report it.

**Responsible disclosure** (also called **coordinated disclosure**) means the researcher privately contacts the vendor, gives them a reasonable time (typically 90 days) to release a patch, and only then publishes details. Google's Project Zero team follows this approach.

**Full disclosure** means publishing the vulnerability immediately, without advance notice. Advocates argue it pressures vendors to act quickly. Critics argue it gives attackers a roadmap before a patch exists.

**Limited disclosure** involves sharing details with a trusted group (such as the CERT Coordination Center) that can coordinate response without publicizing the flaw. Each approach reflects different ethical priorities: user protection, vendor accountability, or a balance of both.

### Patch Management Ethics

**Patch management** is the process of developing, testing, and distributing updates that fix known vulnerabilities. It raises its own ethical questions: How quickly must a vendor release a patch? How much testing is required before deployment (a hasty patch can itself cause problems, as CrowdStrike demonstrated)? What obligation does a vendor have to patch software that has reached "end of life" but is still widely used?

The 2017 Equifax breach exposed the personal information of approximately 147 million people through a vulnerability that had a patch available two months earlier. Equifax knew about it but failed to apply it. The ethical failure was not the existence of the vulnerability. It was the organizational decision-making that left a known flaw unpatched in a system holding sensitive personal data.

### Think About It 7.3 🧠

> Imagine you are a security researcher who discovers a critical vulnerability in a widely used open source library. The maintainer of the library is a single volunteer who responds to emails slowly and has no formal patching process. Meanwhile, you know that millions of applications depend on this library. Would you follow responsible disclosure (and wait, potentially for months, while users remain vulnerable), or would you choose a different approach? What factors would influence your decision?

### Quick Check 7.3 ✅

1. In your own words, explain what SQL injection is and why it is dangerous. You do not need to use technical code examples. Focus on the concept and the potential impact. *(Understand)*

2. Compare responsible disclosure and full disclosure of software vulnerabilities. What ethical values does each approach prioritize, and what risks does each approach accept? *(Analyze)*

3. The Equifax breach occurred because a known patch was not applied for two months. Identify at least two organizational factors that might explain why the patch was not applied, and explain whether any of those factors are ethically acceptable excuses. *(Evaluate)*

---

## 7.4 Cost/Benefit Analysis and Safety-Critical Systems

Every IT decision involves trade-offs. Cost/benefit analysis is a legitimate and necessary tool. But when that analysis is applied to decisions that affect human safety, the ethical stakes increase dramatically.

### Risk Assessment Frameworks in IT

**Risk assessment** is the systematic process of identifying potential threats and estimating their likelihood and impact. The standard formula:

**Risk = Likelihood x Impact**

A very likely threat with minimal impact (a minor website glitch) receives lower priority than an unlikely but catastrophic one (a complete data center failure). The **NIST Risk Management Framework** provides structured processes for evaluating and prioritizing risks.

**Cost/benefit analysis** weighs the cost of a security measure or improvement against the expected benefit, usually expressed as reduced risk. If a $50,000 security upgrade reduces expected annual losses from breaches by $200,000, the calculation favors the investment.

### The Ethical Dimensions of Cost/Benefit Analysis

Cost/benefit analysis becomes ethically problematic when it reduces human safety, privacy, or well-being to a dollar figure. The most infamous example is the Ford Pinto case: Ford calculated that paying settlements for burn injuries and deaths was cheaper than a recall. The math may have been accurate. The ethics were indefensible.

Similar reasoning appears in IT. An organization might calculate that the cost of a comprehensive security audit exceeds the expected financial loss from a breach, and conclude that skipping it is "rational." But this omits what is difficult to quantify: the human suffering caused by identity theft, the erosion of public trust, and the disproportionate impact on vulnerable populations with fewer resources to recover from fraud.

Ethical cost/benefit analysis requires acknowledging what the numbers leave out:

* **Who bears the risk?** The people who benefit from cost savings (executives, shareholders) are often not the people who suffer when things go wrong (users, patients, the public). When risk-bearers and decision-makers are different groups, there is an ethical obligation to give extra weight to those who bear the risk.

* **What is being valued?** A patient whose medical records are exposed suffers harm that credit monitoring services cannot fully address.

* **What alternatives exist?** Cost/benefit analysis is useful when comparing options. It becomes dangerous when used to frame the cheapest option as the only "rational" choice.

### Safety-Critical Systems

A **safety-critical system** is any system whose failure could result in death, serious injury, or significant environmental damage. Examples include aviation software, medical devices, nuclear power plant controls, autonomous vehicle systems, and industrial control systems.

Safety-critical systems demand a fundamentally different approach to quality and testing. The standard of "good enough" for a social media app is wholly inadequate for software controlling a passenger aircraft. Key principles include:

* **Redundancy:** Critical functions are backed by independent secondary systems.
* **Formal verification:** Mathematical methods prove that software meets its specifications.
* **Certification standards:** Aviation software follows DO-178C; medical device software follows IEC 62304; automotive software follows ISO 26262.
* **Fail-safe design:** When a safety-critical system encounters an error it cannot handle, it defaults to a safe state rather than continuing to operate unpredictably.

When failure means someone could die, the obligation to get it right is not measured by cost/benefit analysis. It is measured by the duty to protect human life.

### AI Liability: Who Is Responsible When AI Causes Harm?

As you explored in Module 3, AI ethics principles (fairness, transparency, accountability, explainability, and human oversight) establish the framework for AI accountability. Module 7 applies that accountability question to liability specifically.

When traditional software causes harm, there is usually a clear chain: the developer wrote the code, the company shipped the product, the failure can be traced to specific decisions. AI complicates this chain in several ways:

* **Opacity:** Many AI systems, particularly deep learning models, operate as "black boxes." Developers may not be able to explain why a system produced a particular output, making it impossible to identify a "defect" in the traditional sense.

* **Training data:** AI systems learn from data. If that data is biased or unrepresentative, the outputs will reflect those flaws. Who is liable: the team that collected the data, the team that built the model, or the organization that deployed it without adequate testing?

* **Evolving behavior:** Some AI systems continue to learn after deployment. A system that performs well during testing may behave differently after months of real-world interaction, challenging the assumption that a product's behavior is fixed at the time of sale.

* **Multiple parties:** An AI system might involve a foundation model built by one company, fine-tuned by a second, deployed by a third. When harm occurs, liability could fall on any of them. Current law does not provide clear answers.

Organizations that rush AI systems to market without adequate testing are making the same ethical error as those that ship software with known defects: transferring risk to users for their own benefit.

### Think About It 7.4 🧠

> Self-driving vehicle companies argue that autonomous cars do not need to be perfect; they only need to be safer than human drivers. If a self-driving car is statistically involved in fewer accidents per mile than a human driver, is that sufficient to justify deployment, even knowing that the AI will still cause some deaths? Who should make that decision: the company, government regulators, or the public? And if an autonomous vehicle does cause a death, who should be held liable: the manufacturer, the software developer, the owner, or no one?

### Quick Check 7.4 ✅

1. Explain the formula "Risk = Likelihood x Impact" and give an example of an IT risk scenario where a low-likelihood, high-impact threat should receive priority attention. *(Apply)*

2. The Ford Pinto case involved a company calculating that paying for injuries was cheaper than fixing a defect. Identify a parallel ethical risk in IT cost/benefit analysis and explain why the same logic is ethically problematic in a technology context. *(Analyze)*

3. An AI-powered hiring tool is found to systematically rank female candidates lower than male candidates with identical qualifications. Using the AI liability concepts from this section, identify at least two parties who might bear responsibility and explain why assigning liability is more complex for AI than for traditional software. *(Evaluate)*

---

## 7.5 Skills Lab 7A - Software Liability and Cost/Benefit Analysis

**Goal:** Analyze a software liability scenario involving safety-critical systems, apply product liability and cost/benefit frameworks, and develop a justified recommendation that balances business interests with ethical obligations.

**Estimated time:** 90-120 minutes

### Scenario: The AutoPilot Express Decision

TransitTech Inc. develops software for autonomous public transit buses operating in Phoenix, Arizona. Their system, AutoPilot Express, has been in pilot testing on two routes for 18 months. The pilot has been largely successful: the buses have completed over 50,000 trips with no serious incidents.

TransitTech is now pursuing a major contract with Valley Metro to expand AutoPilot Express to 15 additional routes across the metropolitan area. The contract is worth $45 million over five years and would make TransitTech the first company to operate autonomous transit at this scale in the United States.

During final pre-deployment testing, a quality assurance engineer named Tomoko Hayashi identifies a pattern: in heavy monsoon rain conditions (common in Phoenix from June through September), the system's sensor fusion algorithm occasionally misidentifies large puddles as solid obstacles, causing the bus to brake abruptly. In 0.3% of simulated heavy rain scenarios, the bus brakes so suddenly that standing passengers would be thrown forward. In 0.05% of those scenarios, the braking force is severe enough to cause injuries comparable to a low-speed car accident.

Tomoko's report also notes that the sensor fusion issue does not occur in light rain or dry conditions (which represent 95% of annual operating conditions in Phoenix). Fixing the issue would require a fundamental redesign of the sensor fusion algorithm, delaying deployment by 8-12 months and costing approximately $6 million in additional development.

TransitTech's leadership team is divided:

* **CEO Maria Santos** wants to proceed with deployment on schedule. She argues that the 0.3% occurrence rate in a condition that represents only 5% of operating days makes the actual risk extremely low. She proposes adding a policy that the buses operate in manual mode during monsoon warnings, which would reduce (but not eliminate) passenger exposure to the defect.
* **CTO James Okonkwo** wants to delay deployment to fix the sensor fusion issue. He argues that TransitTech is setting a precedent for the entire autonomous transit industry, and that a single injury could set public acceptance of autonomous vehicles back by years.
* **CFO Patricia Reeves** presents a financial analysis: the 8-12 month delay would cost $6 million in development plus $3.2 million in lost revenue from the delayed contract, and risks losing the contract entirely to a competitor.
* **Tomoko Hayashi (QA engineer)** has documented the defect and presented her findings. She believes the manual mode policy is a reasonable mitigation but worries about the scenarios where monsoon conditions develop rapidly and buses are already in autonomous mode.

### Part 1: Foundation (Aligns with LO1)

Apply product liability concepts to this scenario:

1. If a passenger is injured due to the abrupt braking defect during a monsoon, which product liability theory (negligence, strict liability, or breach of warranty) would most likely apply? Explain your reasoning, referencing the fact that TransitTech knows about the defect before deployment.

2. Would the manual mode policy during monsoon warnings change the liability analysis? Why or why not?

3. Identify whether AutoPilot Express should be classified as a safety-critical system. Reference the characteristics of safety-critical systems discussed in Section 7.4 to support your answer.

### Part 2: Application (Aligns with LO2)

Analyze the ethical obligations of the development team and organization:

4. Evaluate the quality of TransitTech's development process. Based on what you know about the scenario, what CMMI maturity level (1-5) does their process most closely resemble? Justify your assessment.

5. Consider Tomoko's position. She has reported the defect to leadership and they have acknowledged it. Does she have any further ethical obligation? If TransitTech proceeds with deployment over her objections, what options does she have? Reference the whistleblowing concepts from Module 5 if relevant.

6. Analyze the CEO's proposed mitigation (manual mode during monsoon warnings). Is this an adequate response to the identified risk, or is it a rationalization that allows the company to proceed while shifting risk to passengers? Explain your reasoning.

### Part 3: Extension (Aligns with LO3)

Evaluate the cost/benefit trade-offs and formulate a recommendation:

7. Construct a cost/benefit analysis that includes both the financial costs (delay, development expense, lost revenue) and the non-financial costs (passenger safety risk, public trust, industry precedent, legal liability). Which factors are most difficult to quantify, and why does that difficulty matter for ethical decision-making?

8. Write a recommendation (200-300 words) to TransitTech's board of directors. State whether they should deploy on schedule, deploy with the manual mode mitigation, or delay to fix the defect. Support your recommendation with at least two ethical frameworks and reference specific concepts from this module.

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

## 7.6 Summary and Retrieval 💡

### Key Concepts

* **Software defects cause real harm.** From the Therac-25 radiation deaths to the 2024 CrowdStrike global outage, software failures range from financial disruption to loss of life. Ethical responsibility extends beyond writing functional code to writing safe, reliable, and secure code.

* **Product liability law applies unevenly to software.** Negligence, strict liability, and breach of warranty provide frameworks for accountability, but the product-vs.-service distinction and EULA protections leave significant gaps. Software vendors often enjoy less legal accountability than manufacturers of physical products.

* **Software quality is an ethical obligation.** Development methodologies (waterfall, agile, DevOps) shape quality outcomes. CMMI provides a maturity framework for assessing organizational capability. Technical debt transfers risk from organizations to users when shortcuts are taken without plans to address them.

* **Secure coding prevents foreseeable harm.** Vulnerabilities like SQL injection, XSS, and authentication flaws are well-understood and preventable. Responsible disclosure, patch management, and ongoing security maintenance are ethical obligations throughout a product's lifecycle.

* **Cost/benefit analysis requires ethical guardrails.** Financial calculations that reduce human safety and privacy to dollar figures are incomplete and potentially dangerous. When failure means serious harm, "good enough" is not good enough.

* **AI liability is an emerging and unresolved challenge.** Opacity, biased training data, evolving post-deployment behavior, and multi-party development chains make it difficult to assign responsibility when AI causes harm. Ethical AI deployment requires rigorous testing, transparent limitations, and clear accountability structures.

### Key Terms

* **Software defect (bug):** An error or unintended behavior in software that causes incorrect or unexpected results.
* **Product liability:** Legal framework holding manufacturers responsible for harm caused by defective products.
* **Negligence:** Liability based on failure to exercise reasonable care in developing or maintaining software.
* **Strict liability:** Liability for a defective product regardless of how much care the manufacturer exercised.
* **Breach of warranty:** Liability when a product fails to perform as expressly or implicitly promised.
* **End User License Agreement (EULA):** A contract between a software provider and user that defines terms of use and typically limits the provider's liability.
* **Software as a Service (SaaS):** A model where applications are hosted in the cloud and accessed via subscription.
* **Software quality:** The degree to which software meets specified requirements and user needs, including reliability, security, and usability.
* **Capability Maturity Model Integration (CMMI):** A framework measuring the maturity of an organization's software development processes across five levels.
* **Technical debt:** The accumulated cost of development shortcuts that create future maintenance, security, and reliability burdens.
* **Secure coding:** Writing software resistant to security vulnerabilities by design, treating inputs and connections as potentially hostile from the start.
* **OWASP Top 10:** A regularly updated list from the Open Web Application Security Project identifying the most critical web application security risks.
* **SQL injection:** A vulnerability where an attacker inserts malicious database commands through unvalidated input fields.
* **Cross-site scripting (XSS):** A vulnerability allowing attackers to inject malicious scripts into web pages viewed by other users.
* **Responsible disclosure:** Privately reporting a vulnerability to the vendor and allowing time for a fix before public disclosure.
* **Patch management:** The process of developing, testing, and distributing software updates that fix known vulnerabilities.
* **Risk assessment:** A systematic process for identifying, evaluating, and prioritizing threats based on likelihood and impact.
* **Cost/benefit analysis:** Evaluating decisions by comparing financial and non-financial costs against expected benefits.
* **Safety-critical system:** A system whose failure could result in death, serious injury, or significant environmental damage.
* **AI liability:** The legal and ethical question of who is responsible when an artificial intelligence system causes harm.

### Retrieval Practice

Try to answer these from memory before looking back at the module.

1. Name and explain the three product liability theories that can apply to software failures. For each one, give an example of a software scenario where that theory would most likely apply.

2. What is technical debt, and why is it an ethical concern rather than just a technical or business concern?

3. Explain why assigning liability for AI-caused harm is more complex than assigning liability for traditional software failures. Identify at least two factors that complicate AI liability.

---

## 7.7 Discussion Prompt 💬

**Prompt:** In 2017, the Equifax data breach exposed the personal information of approximately 147 million people. The breach exploited a known vulnerability in the Apache Struts framework for which a patch had been available for two months. Equifax's eventual settlement included up to $425 million in consumer relief, but critics argued this amounted to roughly $3 per affected person.

Should software companies face strict liability for data breaches caused by their failure to apply known security patches within a reasonable timeframe? Or should the current system, where liability depends on proving negligence and is often limited by EULAs, remain in place?

Take a clear position and support it using at least one concept from this module (product liability theory, cost/benefit analysis, software quality obligations, or secure coding principles). Then address the strongest counterargument to your position.

**Guidelines:**
* Your initial post should be 200-300 words
* Reference at least one ethical framework or concept from this module
* Respond to at least two classmates with substantive engagement

---

## Further Reading 📖

* **OWASP Foundation: "OWASP Top 10."** The definitive and regularly updated list of the most critical web application security risks. Free online at owasp.org. Essential reference for anyone involved in software development or security.

* **Leveson, N. (2020). "Engineering a Safer World."** An open access book from MIT Press examining system safety engineering and its application to software-intensive systems. Chapters on the Therac-25 case and safety-critical system design are particularly relevant to this module.

* **NIST Special Publication 800-30: "Guide for Conducting Risk Assessments."** A free, comprehensive guide from the National Institute of Standards and Technology on risk assessment methodology. Useful for understanding how organizations evaluate and prioritize IT risks.

* **Krebs, B. (2024). "What We Know About the CrowdStrike Update Crash."** Journalism covering the July 2024 CrowdStrike incident, including technical details and industry analysis. Available at krebsonsecurity.com.

* **European Commission: "Proposal for an AI Liability Directive."** The EU's proposed framework for assigning liability when AI systems cause harm. Represents one of the most developed regulatory approaches to AI liability globally. Free to read at ec.europa.eu.

---

## Looking Ahead ⏩

In Module 8, you will shift from the obligations of those who build software to the role of governments and professional organizations in regulating IT. You will examine major regulations including GDPR, CCPA, COPPA, and HIPAA, evaluate the tension between government regulation and industry self-regulation, and explore the ethical dimensions of H-1B visa programs and offshore outsourcing. The question changes from "What should developers do?" to "What should society require?"
