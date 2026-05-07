# Module 11: Cybersecurity, Identity Theft, and Risk Assessment

In December 2020, the U.S. government disclosed that sophisticated attackers had compromised SolarWinds, whose Orion network monitoring software was used by more than 30,000 organizations including Treasury, DHS, and Fortune 500 companies. The attackers had inserted malicious code into a routine software update months earlier and moved undetected through government and corporate networks for at least nine months, reading emails, accessing files, and exfiltrating data. None of the affected organizations found the breach; cybersecurity firm FireEye discovered it only after attackers compromised FireEye itself.

SolarWinds illustrates a sobering reality: even well-resourced organizations with dedicated security teams can be breached. For IT professionals, knowing how to protect systems, respond to incidents, and build security policies is core professional responsibility.

This module covers the broadest range in the course because cybersecurity sits at the intersection of technology, law, policy, and ethics. You will learn the CIA Security Triad, examine identity theft and federal cybercrime laws, study real breach cases and risk-assessment frameworks, and explore how organizations build security policies and respond to incidents, including how AI is reshaping both sides of the equation.

## Module Overview 🧭

* **Estimated time:** 5-6 hours (reading + activities + discussion)
* **Prerequisites:** Modules 1-10
* **Deliverables:** Discussion post, Quick Checks, Skills Lab analysis
* **CLOs addressed:** CLO XIV, CLO XV, CLO XVI, CLO XVIII

### Module Learning Objectives *(MLO)* 🎯

By the end of this module, **you will be able to**:

* MLO-11.1 (Analyze): **Analyze major identity theft methods and evaluate the effectiveness of prevention and response strategies** *(CLO XIV)*
* MLO-11.2 (Evaluate): **Evaluate IT security breaches using the CIA Security Triad and risk assessment frameworks to identify what went wrong and how threats should be prioritized** *(CLO XV, CLO XVIII)*
* MLO-11.3 (Create): **Formulate security policies and develop prevention, detection, and response procedures for IT security threats** *(CLO XVI, CLO XVIII)*

---

## 11.1 The CIA Security Triad and the Threat Landscape

Every cybersecurity decision connects back to three principles. Whether you configure a firewall, write a policy, or respond to a breach, they tell you what you are protecting and why.

### The CIA Security Triad

The **CIA Security Triad** is the foundational framework for information security:

* **Confidentiality** keeps information accessible only to authorized users. A hospital restricting patient records to medical staff protects confidentiality; a hacker stealing a database of Social Security numbers breaches it.
* **Integrity** keeps information accurate, complete, and untampered. A bank guaranteeing your account balance reflects actual transactions protects integrity; an attacker altering financial records or modifying a software update (as in SolarWinds) compromises it.
* **Availability** keeps information and systems accessible to authorized users when needed. A hospital EHR operational during an emergency has availability; ransomware locking down a city's systems destroys it.

These principles often trade against each other. Maximizing confidentiality (complex authentication for every action) reduces availability. Maximizing availability (easy access from anywhere) reduces confidentiality. Effective security balances all three based on the organization's risk tolerance.

### Implementing CIA at Multiple Levels

Organizations implement CIA at four levels:

**Organizational level.** Clear governance, defined roles, security budgets, and a culture that treats security as everyone's responsibility. Module 3's corporate-governance principles apply: leadership that underfunds security or ignores warnings puts stakeholders at risk.

**Network level.** Firewalls, **intrusion detection systems (IDS)**, **intrusion prevention systems (IPS)**, **virtual private networks (VPNs)**, and network segmentation protect data in transit and monitor for suspicious activity.

**Application level.** Secure coding (Module 7), input validation, authentication, and encryption protect individual applications. SQL injection and cross-site scripting remain among the most common attack vectors.

**End-user level.** The human element is consistently the weakest link. Strong passwords, **multi-factor authentication (MFA)**, security awareness training, and clear acceptable use policies help protect against social engineering and phishing. No technical infrastructure compensates fully for a user who clicks a malicious link.

### The Current Threat Landscape

Why are computer incidents so prevalent? Several factors converge:

* **Expanding attack surface.** Every new device, application, cloud service, and **Internet of Things (IoT)** sensor is another entry point. Organizations now manage thousands of connected endpoints.
* **Professionalization of cybercrime.** Organized criminal groups operate like businesses with specialized roles and customer service for ransomware victims. **Ransomware as a Service (RaaS)** lets criminals with limited skills launch devastating attacks using tools developed by others.
* **Nation-state actors.** Russia, China, North Korea, and Iran conduct cyber operations for espionage, sabotage, and strategic advantage. The SolarWinds attack is attributed to Russia's SVR. Their resources and patience exceed typical criminal organizations.
* **The speed gap.** Once a vulnerability is discovered, attackers develop **exploits** within hours or days; many organizations take weeks or months to apply patches.
* **Human factors.** Social engineering, phishing, and credential theft exploit psychology rather than technical flaws and are involved in most successful breaches.

Common types of exploits include:

| Exploit Type | How It Works | CIA Impact |
|---|---|---|
| **Phishing** | Deceptive emails or messages trick users into revealing credentials or installing malware | Confidentiality |
| **Ransomware** | Malware encrypts data and demands payment for the decryption key | Availability, Integrity |
| **Distributed Denial of Service (DDoS)** | Overwhelms systems with traffic to make them unavailable | Availability |
| **SQL injection** | Inserts malicious database commands through application input fields | Confidentiality, Integrity |
| **Man-in-the-middle (MITM)** | Intercepts communication between two parties without their knowledge | Confidentiality, Integrity |
| **Zero-day exploit** | Targets a previously unknown vulnerability before a patch is available | All three |
| **Insider threat** | An authorized user intentionally or accidentally causes harm | All three |

### Think About It 11.1 🧠

> Think about the devices and accounts you use every day: your phone, email, social media, banking apps, school accounts. How many of these use multi-factor authentication? How many share the same password? If an attacker compromised one of your accounts today, what other accounts or data could they reach from there?

### Quick Check 11.1 ✅

1. Explain the three components of the CIA Security Triad and give one example of how each can be compromised. *(Understand)*

2. A university stores student grades in a cloud-based system. During final exams week, a DDoS attack makes the system inaccessible for 12 hours. Which component of the CIA triad was primarily compromised, and what secondary impacts might this have on the other two components? *(Analyze)*

3. Why is the "speed gap" between vulnerability discovery and patch deployment such a persistent cybersecurity challenge? Identify at least two reasons organizations struggle to close this gap. *(Analyze)*

---

## 11.2 Identity Theft and Cybercrime

Identity theft is one of the most personal consequences of cybersecurity failures. Victims spend months or years restoring credit, correcting fraudulent records, and recovering from the emotional toll. Understanding how it works is essential for IT professionals who protect the systems where personal data lives.

### What Is Identity Theft?

**Identity theft** is the unauthorized use of another person's **personally identifiable information (PII)**, typically for financial gain. PII includes names, Social Security numbers, dates of birth, addresses, and financial account numbers.

Identity theft takes several forms:

* **Financial identity theft** (most common): the thief opens credit cards, takes out loans, or makes purchases in the victim's name.
* **Medical identity theft**: someone uses another person's identity to obtain medical care, prescriptions, or insurance benefits, creating false medical records that can lead to dangerous treatment decisions.
* **Criminal identity theft**: someone provides another person's identity during an arrest, leaving the victim with a criminal record they know nothing about.
* **Synthetic identity theft** (growing): criminals combine real and fabricated information, often pairing a real Social Security number (often a child's or a deceased person's) with a fake name and address. Synthetic identities are hard to detect because they do not match any existing person's records.
* **Tax identity theft**: filing a fraudulent return using someone else's SSN to claim their refund.

### Methods and Scale

Thieves obtain PII through multiple channels:

* **Data breaches** expose millions of records at once. The 2017 Equifax breach (Module 7) compromised data on approximately 147 million people.
* **Phishing and social engineering** trick individuals into voluntarily providing information through convincing emails, fake websites, or phone calls.
* **Dumpster diving and mail theft** remain effective: financial statements, pre-approved credit card offers, and medical bills all contain valuable PII.
* **Skimming** uses devices attached to ATMs or point-of-sale terminals to capture card data during legitimate transactions.
* **Dark web marketplaces** sell stolen identities, credit card numbers, and login credentials in bulk. A stolen SSN sells for a few dollars; a complete identity package can sell for significantly more.

The FTC receives millions of identity theft reports each year, and the actual number is likely much higher because many cases go unreported.

### Prevention and Response

Prevention requires action at both individual and organizational levels:

**Individual:**

* Strong, unique passwords and MFA wherever possible
* Regular credit monitoring (free annual reports from AnnualCreditReport.com)
* Credit freezes at Equifax, Experian, and TransUnion
* Caution about sharing personal information in response to unsolicited requests
* Shredding documents containing PII before disposal

**Organizational:**

* Collect only PII that is genuinely necessary (data minimization)
* Encrypt PII at rest and in transit
* Apply access controls so employees see only data they need
* Conduct regular security audits and vulnerability assessments
* Maintain a breach notification plan before a breach occurs
* Train employees to recognize social engineering

**If identity theft occurs,** the FTC sequence: place a fraud alert on credit reports, review for unfamiliar accounts, report at IdentityTheft.gov, file a police report, and contact fraud departments of affected companies. Recovery takes months and requires persistent follow-up.

### Federal Laws for Prosecuting Cybercrime

Several federal laws frame the prosecution of identity theft and computer crimes:

* **Computer Fraud and Abuse Act (CFAA)**: The primary federal law for computer crimes. Passed in 1986 and amended repeatedly, it criminalizes unauthorized access, exceeding authorized access, trafficking in passwords, and transmitting malicious code. Critics argue its broad language can criminalize minor activities like violating a website's terms of service.
* **Identity Theft and Assumption Deterrence Act (1998)**: Made identity theft a federal crime and established penalties for using another person's identification to commit a crime.
* **Electronic Communications Privacy Act (ECPA)**: Governs interception of electronic communications, including the Wiretap Act and Stored Communications Act. Critics argue ECPA offers weaker protections for stored data than for real-time communications and has not kept pace with technology.
* **CAN-SPAM Act (2003)**: Establishes rules for commercial email and gives recipients the right to opt out. Relevant to cybersecurity because phishing campaigns often violate it.
* **State breach notification laws**: All 50 states now have them, but specific requirements (what counts as a breach, notification timeline, required content) vary widely.

### Think About It 11.2 🧠

> The CFAA's broad language has led to debates about whether activities like sharing a password with a friend or using a work computer for personal tasks could technically be federal crimes. Where do you think the line should be between legitimate security protection and overcriminalization of everyday computer use?

### Case Study 11.1 - The Anthem Healthcare Breach 📋

**The Situation:** In February 2015, Anthem, Inc., the second-largest health insurer in the United States, disclosed that attackers had breached its systems and stolen the personally identifiable information of approximately 78.8 million current and former members and employees. The stolen data included names, dates of birth, Social Security numbers, home addresses, email addresses, and employment information. Notably, the breach did not compromise medical records or financial data, but the scope of PII exposed was extraordinary.

The investigation revealed that the attackers had gained access through a spear phishing email sent to an Anthem employee. The email contained a malicious link that, when clicked, installed malware that allowed the attackers to move through Anthem's network and eventually access a database warehouse containing years of member information. The attackers had been inside the network for weeks before detection.

Several factors compounded the severity. Anthem had not encrypted the Social Security numbers stored in the compromised database. The company argued that encryption would have been impractical given the volume of data that needed to be accessed for daily business operations. Critics responded that this decision prioritized operational convenience over the protection of highly sensitive data. Anthem ultimately agreed to a $115 million class-action settlement and a $16 million settlement with the U.S. Department of Health and Human Services for HIPAA violations.

**Stakeholders:**

* **78.8 million members and employees** whose PII was stolen, creating long-term identity theft risk
* **Anthem leadership and IT security team** who made decisions about encryption, access controls, and phishing defenses
* **Healthcare providers and partners** who relied on Anthem's data security for patient trust
* **Federal and state regulators** responsible for enforcing data protection standards
* **The broader healthcare industry** which faced increased scrutiny of data security practices following the breach

**Questions to Consider:**

1. Anthem argued that encrypting the database was impractical for daily operations. Using the CIA triad, analyze whether this decision was a reasonable trade-off between availability and confidentiality, or an unjustifiable risk to member data.

2. The breach began with a single phishing email. To what extent should Anthem be held responsible for an employee's action, and what organizational measures could have limited the damage even after the initial compromise?

3. If you were an IT professional at Anthem who had recommended encryption of the database but was overruled by management, what would you do after the breach became public? Consider the whistleblowing principles from Module 5 and the fiduciary responsibilities discussed there.

### Quick Check 11.2 ✅

1. Name and briefly describe three different forms of identity theft. *(Remember)*

2. The CFAA criminalizes "unauthorized access" and "exceeding authorized access" to computer systems. Explain why the broad language of these terms has been controversial. *(Understand)*

3. An organization stores customer Social Security numbers in an unencrypted database because encrypting it would slow down their claims processing system. Using the CIA triad, analyze this decision. Which principle did they prioritize, and which did they sacrifice? *(Analyze)*

---

## 11.3 Security Breaches, Risk Assessment, and Security Policies

Major data breaches almost always reveal a chain of decisions, oversights, and systemic failures rather than a single moment of catastrophic error. Understanding what goes wrong, how to assess risk, and how to build security policies are interconnected skills that define competent IT security practice.

### IT Security Breaches: What Goes Wrong and Why

Common breach factors:

* **Unpatched vulnerabilities.** The 2017 Equifax breach exploited a known Apache Struts flaw for which a patch had been available for two months.
* **Weak access controls.** The 2013 Target breach began with compromised credentials from a third-party HVAC vendor; attackers moved laterally to point-of-sale systems because the network was not properly segmented, stealing approximately 40 million card numbers.
* **Inadequate monitoring.** Attackers often operate inside networks for weeks or months before detection. The SolarWinds attackers had access for at least nine months.
* **Insufficient encryption.** As the Anthem case study shows, unencrypted data at rest means a breach of access controls immediately exposes data in readable form.
* **Human error.** Misconfigured cloud buckets, accidental email disclosures, lost devices, and weak passwords cause many breaches; these are preventable mistakes, not sophisticated attacks.
* **Third-party risk.** Vendors, cloud providers, and software supply chains are entry points. SolarWinds exploited this explicitly through a trusted software provider.

### Risk Assessment Frameworks

**Risk assessment** systematically identifies, analyzes, and evaluates threats to information assets, helping organizations prioritize security investment where it matters most.

Standard steps:

1. **Asset identification.** What are you protecting? Data, systems, applications, IP, and physical infrastructure. A database of customer SSNs requires more protection than a marketing website.
2. **Threat identification.** External attackers, insider threats, natural disasters, hardware failures, and software defects.
3. **Vulnerability assessment.** Vulnerability scanning, penetration testing, and security audits reveal weaknesses.
4. **Likelihood estimation.** Historical data, industry intelligence, and threat modeling inform estimates.
5. **Impact analysis.** Financial loss, reputational damage, regulatory penalties, operational disruption, and harm to individuals.
6. **Risk calculation.** **Risk = Likelihood x Impact.** High-likelihood, high-impact threats demand immediate attention.
7. **Risk response.** Mitigate (reduce likelihood or impact), transfer (e.g., cyber insurance), accept (low-priority risks), or avoid (eliminate the risky activity).

The **NIST Cybersecurity Framework** organizes security functions into five categories, Identify, Protect, Detect, Respond, Recover, and has become a de facto standard, particularly for organizations working with the U.S. government.

### Think About It 11.3 🧠

> Think about a small business you are familiar with, such as a local restaurant, a tutoring service, or a small retail shop. What digital assets does that business have (customer data, financial records, online ordering systems)? If you were conducting a risk assessment for that business, what would you identify as the three most significant risks? How would your recommendations differ from those for a large corporation?

### Formulating Security Policies

A **security policy** is a formal document defining an organization's rules and procedures for protecting information assets. Policies translate CIA principles and risk-assessment findings into actionable guidelines.

Effective policies address several areas:

* **Acceptable use policy (AUP):** What employees can and cannot do with organizational technology, including personal-device-for-work rules (**BYOD**).
* **Password and authentication:** Complexity, expiration, and MFA requirements. Weak passwords remain a primary attack vector.
* **Data classification and handling:** Categorizes data by sensitivity (public, internal, confidential, restricted) and defines storage, transmission, and disposal for each. A **data classification** policy ensures a customer's SSN gets stronger protection than a company newsletter.
* **Access control:** Implements the **principle of least privilege**, granting users access only to data and systems necessary for their job. Limits damage from compromised credentials or insider threats.
* **Incident response:** What happens when a security incident occurs (Section 11.4).
* **Remote work and mobile device:** Security for employees working from home or using mobile devices. Far more critical post-2020.
* **Vendor and third-party risk management:** Security requirements for partners with access to data or systems. Target and SolarWinds both demonstrate the consequences of inadequate vendor management.

### Policy Enforcement and Compliance

A policy on paper provides no protection. Enforcement requires:

* **Training and awareness.** Annual security awareness training at minimum; strong security cultures provide ongoing education.
* **Technical controls.** Enforce through technology where possible: if password policy requires 12 characters, the system should reject shorter passwords.
* **Monitoring and auditing.** Audits verify compliance. This raises workplace monitoring tensions from Module 10; transparent policies stating what is monitored and why help balance security with employee privacy.
* **Consequences for violations.** Clear, consistent consequences. If executives are exempt, policies lose credibility.
* **Regular review.** The threat landscape changes constantly; review at least annually and after significant incidents.

### Quick Check 11.3 ✅

1. List the four possible responses to an identified risk in a risk assessment framework and give a brief example of when each would be appropriate. *(Remember)*

2. Explain the principle of least privilege and describe how violating it contributed to a real breach discussed in this module. *(Understand)*

3. A company drafts a strict security policy requiring complex passwords, mandatory encryption, and limited remote access. However, employees routinely bypass these controls because they slow down daily work. What does this situation reveal about the relationship between security policies and organizational culture? What would you recommend? *(Evaluate)*

---

## 11.4 Incident Response, Computer Forensics, and AI in Cybersecurity

No matter how strong policies and controls are, breaches occur. The question is not whether but how prepared you are.

### The Incident Response Lifecycle

**Incident response** is the organized approach to managing a security breach or cyberattack: limit damage, reduce recovery time and cost, and preserve evidence for legal proceedings. The NIST framework defines four phases:

**Phase 1: Preparation.** Before any incident: form an incident response team, define roles, establish communication channels, create playbooks, and run regular tabletop exercises. Organizations without a prepared plan make costly mistakes under active-breach pressure.

**Phase 2: Detection and analysis.** Often the hardest phase. **Security information and event management (SIEM)** systems, intrusion detection, **endpoint detection and response (EDR)** tools, and alert monitoring contribute to detection. Once detected, the team analyzes scope, severity, and nature: is this one user phished, or a network-wide compromise?

**Phase 3: Containment, eradication, and recovery.** Contain (prevent spread), eradicate (remove the attacker and malicious code), recover (restore normal operations). Short-term containment isolates affected segments; long-term containment may require rebuilding compromised systems. Verify recovery through testing before returning systems to production.

**Phase 4: Post-incident activity.** Review: what happened, how it was detected, what worked, what needs improvement. The "lessons learned" process strengthens defenses for next time and includes documentation for legal, regulatory, and insurance purposes.

### Notification and Legal Obligations

When a breach involves personal data, organizations face legal notification requirements. All 50 states have breach notification laws with varying specifics:

* **Who must be notified?** Affected individuals; many laws also require state AGs, the FTC, or industry-specific regulators (HHS for health data, per Module 6's HIPAA discussion).
* **How quickly?** 30 to 90 days in most states; some require "as expeditiously as possible." Delays bring additional penalties and erode trust.
* **What must it include?** What happened, what data was compromised, what the organization is doing, and what affected individuals should do.

The ethical obligation extends beyond the law. Even when not legally required, the question is whether people whose data was exposed have a right to know. Grounded in Module 5's fiduciary principles, the answer is almost always yes. Transparency protects individuals and preserves trust.

### Computer Forensics

**Computer forensics** (or **digital forensics**) collects, preserves, analyzes, and presents digital evidence in a legally admissible way. After a breach, it answers: who did this, how did they get in, what did they access, how long were they inside?

Evidence integrity depends on strict procedures:

* **Preservation.** Create **forensic images** (exact bit-for-bit copies) before any changes. Shutting down, rebooting, or opening files can destroy evidence. The principle is "collect first, analyze later."
* **Chain of custody.** Document every step: who collected what, when, where, how stored. A break in the **chain of custody** can make evidence inadmissible. Investigators use write blockers (preventing changes to the original) and cryptographic hashes (verifying evidence is unaltered).
* **Analysis.** Examine log files, file systems, network traffic, email, and memory dumps; recover deleted files, trace connections, analyze malware, reconstruct attacker timelines. Tools are specialized; the principle is systematic, methodical investigation.
* **Reporting.** Findings must withstand legal scrutiny. Analysts may testify as expert witnesses; testimony rests on evidence, not speculation.

For non-specialists, the lesson is: do not contaminate the evidence. If you suspect an incident, do not run your own investigation on affected systems. Secure them, document what you observed, and contact the incident response team or a qualified forensic specialist. Well-intentioned actions by untrained personnel are one of the most common ways digital evidence is compromised.

### AI Touchpoint: AI on Both Sides of the Cybersecurity Equation

The same AI capabilities that strengthen defenses empower attackers, creating an escalating arms race.

**AI-powered cyberattacks:**

* **Spear phishing at scale.** AI generates thousands of personalized phishing emails by scraping social media and public records, industrializing what was once labor-intensive.
* **Social engineering automation.** AI chatbots conduct real-time conversational attacks. Voice cloning replicates a specific person's voice from seconds of audio, enabling phone calls that sound like the CEO requesting an urgent wire transfer.
* **AI-generated malware.** LLMs write or modify malicious code, generating variants that evade detection. Vendor safeguards exist; open-source models without them are freely available.
* **Deepfake-enabled fraud.** In 2024, a Hong Kong finance worker transferred roughly $25 million after attending a video call where every other participant, including the CFO, was a deepfake.

**AI in defense:**

* **SOCs** use AI to analyze vast security data, flagging the handful of millions of log entries that represent genuine threats.
* **Behavioral analytics** establish normal-behavior baselines and alert on deviations: an employee who normally works business hours suddenly downloading large volumes at 3 AM gets flagged.
* **Automated response.** AI can isolate a compromised endpoint or block a malicious IP without waiting for humans, critical when attacks spread in minutes.
* **Threat intelligence.** AI predicts emerging threats from global data, dark web activity, and vulnerability databases.

**Limitations:**

* **False positives and alert fatigue.** Too many false alarms cause teams to miss real threats.
* **Adversarial AI.** Attackers can craft inputs that cause AI to misclassify malicious activity as benign.
* **Bias.** AI trained on historical threat data detects familiar patterns better than novel ones, and may flag user behaviors based on demographic correlations.
* **Over-reliance.** AI enhances human analysts; it does not replace them. Organizations that cut teams based on AI find themselves vulnerable to threats AI was not trained for.

### Think About It 11.4 🧠

> The same AI voice cloning technology that enables fraud (replicating a CEO's voice for a fake phone call) also has legitimate uses in accessibility and entertainment. How should society balance the benefits of this technology against its potential for harm? Should there be restrictions on who can use voice cloning tools and for what purposes?

### Quick Check 11.4 ✅

1. List the four phases of the NIST incident response lifecycle and explain why the "preparation" phase, which happens before any incident occurs, is considered the most important. *(Understand)*

2. Explain why an IT professional who discovers a potential security breach should not attempt their own forensic investigation on the affected systems. What specific risks does untrained investigation create? *(Understand)*

3. A company's AI-powered security system flags an employee's activity as suspicious because the employee is accessing files outside normal business hours. The employee, who works a late shift, complains that the system unfairly targets their work pattern. Evaluate the ethical trade-offs between AI-powered behavioral monitoring and employee privacy. What steps could the organization take to address both security and fairness concerns? *(Evaluate)*

---

## 11.5 Skills Lab 11A - Developing an Incident Response Plan

**Goal:** Apply the concepts from this module to develop a comprehensive incident response plan for a realistic organizational scenario, demonstrating your ability to analyze identity theft risks, evaluate security breaches, formulate security policies, and design prevention, detection, and response procedures.

**Estimated time:** 90-120 minutes

### Scenario

MidState Community College (MCC) enrolls approximately 12,000 students and employs 800 faculty and staff. The college's IT infrastructure includes:

* A student information system (SIS) containing student names, Social Security numbers, dates of birth, addresses, financial aid data, and academic records
* A learning management system (LMS) used by all students and faculty
* A cloud-based email system and collaboration platform
* A network of campus computers in labs, offices, and the library
* A public-facing website with an online application and payment portal
* A campus Wi-Fi network accessible to students, employees, and visitors

MCC recently experienced the following incident: A phishing email that appeared to come from the IT help desk was sent to approximately 200 faculty members. The email asked recipients to "verify their credentials" by clicking a link and entering their username and password. Thirty-two faculty members entered their credentials before the phishing attack was identified. During the investigation, the IT team discovered that six of the compromised accounts had been used to access the student information system, potentially exposing the personal data of approximately 4,500 students. The attackers also used two compromised accounts to send additional phishing emails to students, requesting financial information for a fake "emergency scholarship."

### Part 1: Breach Analysis (Aligns with LO1 and LO2)

1. Using the CIA Security Triad, analyze which components were compromised at each stage of this incident (the initial phishing attack, the credential theft, the SIS access, and the secondary phishing campaign targeting students).

2. Identify at least three specific security failures or vulnerabilities that allowed this incident to escalate from a phishing email to a potential breach of 4,500 student records.

3. What forms of identity theft are the 4,500 affected students now at risk for? Be specific about which types of stolen data enable which types of identity theft.

### Part 2: Policy Formulation (Aligns with LO3)

4. Draft three specific security policy recommendations that MCC should implement to prevent a similar incident in the future. For each policy, identify:
   * What the policy requires
   * How it would be technically enforced
   * How it addresses a specific vulnerability revealed by this incident

5. MCC does not currently require multi-factor authentication for any systems. Write a brief policy statement (100-150 words) that establishes an MFA requirement for the college. Specify which systems and user groups it applies to, the timeline for implementation, and any exceptions.

### Part 3: Incident Response Plan (Aligns with LO3)

6. Using the four-phase NIST incident response lifecycle, outline the specific actions MCC should take for this incident:
   * **Preparation:** What should MCC have had in place before this happened?
   * **Detection and analysis:** How should the incident be investigated and scoped?
   * **Containment, eradication, and recovery:** What immediate and long-term actions should be taken?
   * **Post-incident activity:** What should the review process cover?

7. Draft a breach notification letter (150-200 words) to the affected students. Include what happened, what data was potentially exposed, what MCC is doing in response, and what steps students should take to protect themselves. Your letter should be clear, honest, and written for a non-technical audience.

### Rubric

| Criteria | Mastery (5) | Proficiency (4) | Developing (3) | Emerging (2) | Not Evident (1) |
|---|---|---|---|---|---|
| **Stakeholder Analysis** | Identifies all major stakeholders with specific, accurate descriptions of their interests and what each stands to gain or lose | Identifies most stakeholders with reasonable descriptions of their interests | Identifies some stakeholders but descriptions lack specificity or miss key interests | Lists stakeholders without meaningful description of their interests | Missing or inaccurate |
| **Ethical Framework Application** | Applies ethical frameworks accurately with clear reasoning and specific references to scenario details; demonstrates understanding of each framework's logic | Applies frameworks correctly with adequate reasoning and some scenario-specific references | Applies frameworks but with gaps in reasoning or limited connection to the scenario | Attempts to apply frameworks but with significant errors or confusion between them | Missing or not recognizable as framework application |
| **Module Concept Application** | Accurately applies module-specific concepts to the scenario with detailed, well-reasoned analysis that demonstrates mastery of the material | Applies module-specific concepts correctly with adequate reasoning and clear connections to the scenario | References module concepts but application is incomplete or partially inaccurate | Mentions module concepts without meaningful application to the scenario | No application of module concepts attempted |
| **Recommendation Quality** | Recommendation is clear, specific, and well-supported by multiple frameworks with explicit reasoning; addresses counterarguments or competing interests | Recommendation is clear and supported by at least one framework with reasonable justification | Recommendation is present but weakly supported or lacks clear connection to ethical reasoning | Recommendation is vague, generic, or unsupported by ethical reasoning | No recommendation provided |
| **Writing and Professionalism** | Writing is clear, well-organized, and uses ethical and professional terminology accurately throughout; ideas flow logically between sections | Writing is clear with mostly accurate terminology and reasonable organization | Writing is understandable but disorganized or imprecise in terminology use | Writing is unclear, contains frequent errors, or lacks professional tone | Unreadable or off-topic |

### Submission Guidelines

* **Length:** 1,200-1,800 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.
* **Due:** See Canvas calendar for deadline

---

## 11.6 Summary and Retrieval 💡

### Key Concepts

* **The CIA Security Triad is the foundation for all security thinking.** Confidentiality, integrity, and availability must be implemented at organizational, network, application, and end-user levels and balanced via risk assessment.
* **Identity theft is a pervasive and personal consequence of security failures.** Financial, medical, criminal, synthetic, and tax forms all exploit stolen PII. Prevention requires individual (strong passwords, credit monitoring, MFA) and organizational action (data minimization, encryption, access controls). Federal laws (CFAA, Identity Theft and Assumption Deterrence Act, ECPA) frame prosecution.
* **Breaches follow recognizable patterns.** Unpatched vulnerabilities, weak access controls, inadequate monitoring, insufficient encryption, human error, and third-party risk recur across breach analyses.
* **Risk assessment prioritizes security investments.** Identifying assets, threats, vulnerabilities, likelihood, and impact lets organizations allocate limited resources where they matter most. The NIST Cybersecurity Framework provides a widely adopted structure.
* **Security policies translate principles into practice.** Effective policies cover acceptable use, authentication, data classification, access control, incident response, remote work, and vendor management, enforced through training, technical controls, monitoring, and consequences.
* **Incident response requires preparation, not improvisation.** The NIST four-phase lifecycle structures the work; computer forensics preserves evidence under strict legal-admissibility procedures.
* **AI is transforming both attack and defense.** AI-powered phishing, social engineering, malware generation, and deepfake fraud escalate threats; AI threat detection, behavioral analytics, and automated response strengthen defense. Neither side has a permanent advantage, and human judgment remains essential.

### Key Terms

**Section 11.1**
* **CIA Security Triad:** Foundational information-security framework: confidentiality, integrity, availability.
* **Confidentiality:** Information accessible only to authorized users.
* **Integrity:** Information accurate, complete, and unaltered by unauthorized parties.
* **Availability:** Systems and information accessible to authorized users when needed.
* **Exploit:** A tool or technique that takes advantage of a vulnerability to compromise a system.
* **Ransomware as a Service (RaaS):** Criminal business model where ransomware developers sell or lease their tools.
* **Intrusion detection system (IDS):** Monitors network traffic for suspicious activity and alerts administrators.
* **Multi-factor authentication (MFA):** Requires two or more independent verification methods to confirm identity.

**Section 11.2**
* **Identity theft:** Unauthorized use of another person's PII for financial gain.
* **Personally identifiable information (PII):** Data that uniquely identifies an individual (SSN, DOB, account numbers).
* **Synthetic identity theft:** Combining real and fabricated information into a new identity.
* **Computer Fraud and Abuse Act (CFAA):** Primary federal law for unauthorized computer access and related crimes.
* **Electronic Communications Privacy Act (ECPA):** Federal law governing interception of electronic communications.
* **Breach notification laws:** State/federal laws requiring notification when personal data is compromised.

**Section 11.3**
* **Risk assessment:** Systematic process for identifying, analyzing, and evaluating threats to information assets.
* **NIST Cybersecurity Framework:** Framework organizing security into Identify, Protect, Detect, Respond, Recover.
* **Security policy:** Formal document defining rules and procedures for protecting information assets.
* **Principle of least privilege:** Users get access only to data and systems necessary for their job.
* **Data classification:** Categorizing data by sensitivity to determine handling and protection.
* **Acceptable use policy (AUP):** Defines what employees can and cannot do with organizational technology.

**Section 11.4**
* **Incident response:** Organized approach to managing the aftermath of a breach or cyberattack.
* **Computer forensics (digital forensics):** Collecting, preserving, analyzing, and presenting digital evidence in a legally admissible way.
* **Chain of custody:** Documented record of who handled evidence, when, and how it was stored.
* **Forensic image:** Exact bit-for-bit copy of a storage device, preserving evidence without altering the original.
* **Security Operations Center (SOC):** Centralized facility for monitoring, detecting, and responding to threats.
* **Behavioral analytics:** Machine learning to establish normal-behavior baselines and detect anomalies.

### Retrieval Practice

Try to answer these from memory before looking back at the module.

1. Draw or describe the CIA Security Triad and explain how a single incident, such as a ransomware attack, can compromise all three components simultaneously.

2. Name three forms of identity theft, explain how each one works, and identify what type of stolen data enables each form.

3. Outline the four phases of the NIST incident response lifecycle. For each phase, describe one specific action an organization should take.

4. Explain how AI is being used on both the attack and defense sides of cybersecurity. Give one specific example of an AI-powered attack and one specific example of an AI-powered defense.

---

## 11.7 Discussion Prompt 💬

**Prompt:** In 2024, a finance worker at a multinational firm transferred approximately $25 million after attending a video conference call where every other participant, including the company's chief financial officer, was a deepfake generated by artificial intelligence. The worker had initially been suspicious of the request but was convinced by the realistic video call.

This incident raises a fundamental question about cybersecurity policy in the age of AI: traditional security training teaches employees to verify requests through established channels, but what happens when the "established channel" (a live video call with recognized colleagues) can itself be faked?

Consider this question: To what extent should organizations hold employees accountable for falling victim to AI-powered social engineering attacks? Should security policies be redesigned to account for the fact that AI can now convincingly impersonate trusted colleagues in real time? If so, what would those policies look like?

Take a clear position and support it using at least two concepts from this module (the CIA triad, risk assessment, security policy formulation, incident response, or AI-powered threats). Then address the strongest counterargument to your position.

**Guidelines:**
* Your initial post should be 250-350 words
* Reference at least two concepts or frameworks from this module
* Respond to at least two classmates with substantive engagement
* Due: See Canvas calendar for deadline

---

## Further Reading 📖

* **NIST Special Publication 800-61: "Computer Security Incident Handling Guide."** A free, comprehensive guide from the National Institute of Standards and Technology on building and maintaining an incident response capability. Essential reading for anyone involved in security operations.

* **NIST Cybersecurity Framework (CSF).** The full framework document, available free at nist.gov, provides detailed guidance on the Identify, Protect, Detect, Respond, and Recover functions. Widely adopted across industries and a valuable resource for understanding organizational cybersecurity management.

* **Federal Trade Commission: "IdentityTheft.gov."** The FTC's comprehensive resource for identity theft victims, including step-by-step recovery plans and sample letters. Also contains data on identity theft trends and prevention strategies.

* **Krebs, B. "Krebs on Security" (krebsonsecurity.com).** Investigative journalism covering cybersecurity breaches, cybercrime, and security policy. Regularly covers major breach investigations and threat landscape developments in accessible, non-technical language.

* **CISA: "Cybersecurity Best Practices."** The Cybersecurity and Infrastructure Security Agency (CISA) provides free resources, alerts, and best practices guides for organizations of all sizes. Available at cisa.gov.

---

## Looking Ahead ⏩

In Module 12, you shift from protecting systems to the professional obligations of the people who build and manage them. You will study the ACM, IEEE, and (ISC)² codes of ethics, compare what they share and where they differ, examine arguments for and against IT licensing and certification, apply the course's frameworks to emerging technologies, and complete a capstone synthesis project bringing everything together.
