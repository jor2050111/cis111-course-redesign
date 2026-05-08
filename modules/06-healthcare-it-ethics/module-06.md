# Module 6: Healthcare IT Ethics

In February 2024, a ransomware attack struck Change Healthcare, one of the largest health technology companies in the United States. Change Healthcare processes roughly 15 billion healthcare transactions each year, handling insurance claims, pharmacy operations, and payment systems for hospitals and clinics nationwide. The attack shut down claims processing for weeks. Physicians could not get paid. Pharmacies could not verify insurance coverage. Small medical practices that depended on timely reimbursements faced potential closure. The personal health data of over 100 million Americans was compromised. One cyberattack on one company disrupted healthcare delivery across the entire country.

That incident exposed something about modern healthcare: it runs on information technology. EHRs, mobile health apps, telemedicine, clinical decision support tools, and AI-assisted diagnostics are woven into how care is delivered, documented, and paid for. Each of those systems creates ethical questions IT professionals face every day. Who has access to your health data? What happens when a clinical system gives a wrong recommendation? Is it ethical to use AI for treatment decisions when the algorithm may perform differently for different populations?

This module examines those ethical challenges. You will learn the legal foundations of health data privacy, evaluate the risks of mobile and wireless technologies in clinical settings, analyze clinical IT systems and telemedicine, and consider the promise and risk of AI in healthcare, applying the frameworks from Part I where patient safety, privacy, equity, and innovation pull against each other.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + activities + discussion)
* **Prerequisites:** Modules 1-5
* **Deliverables:** Discussion post, Quick Checks, Skills Lab analysis
* **CLOs addressed:** CLO VI

### Module Learning Objectives *(MLO)* 🎯

By the end of this module, **you will be able to**:

* MLO-6.1 (Understand): **Explain the key provisions of HIPAA and the ethical foundations of health data privacy, including Protected Health Information, the Privacy Rule, and the Security Rule** *(CLO VI)*
* MLO-6.2 (Apply): **Apply ethical frameworks to evaluate real-world healthcare IT scenarios involving mobile health technologies, telemedicine, and clinical information systems** *(CLO VI)*
* MLO-6.3 (Analyze): **Analyze the ethical challenges of operating mobile and wireless technologies in healthcare environments, including AI-assisted diagnostics and algorithmic bias in clinical settings** *(CLO VI)*

---

## 6.1 HIPAA and the Foundations of Health Data Privacy

Health data is uniquely sensitive. Your medical records reveal diagnoses, mental health treatment, prescription medications, genetic test results, reproductive decisions, and substance use history. When that information is exposed, the consequences can include discrimination, stigma, job loss, and insurance denial. That sensitivity is why the United States created a specific legal framework for protecting it.

### The Health Insurance Portability and Accountability Act (HIPAA)

Congress passed the **Health Insurance Portability and Accountability Act (HIPAA)** in 1996. Its most significant impact on IT professionals comes from its privacy and security provisions, which set national standards for who can access health data, how it must be protected, and what happens when protection fails.

HIPAA applies to **covered entities**, which include healthcare providers (hospitals, clinics, physicians), health plans (insurance companies, HMOs), and healthcare clearinghouses. It also applies to **business associates**, companies that handle health data on behalf of covered entities. Cloud storage providers, software vendors, billing companies, and IT service firms that work with healthcare organizations are all business associates. If you work in IT and your company touches health data, HIPAA applies to you.

### Protected Health Information (PHI)

**Protected Health Information (PHI)** is the core concept in HIPAA's privacy framework: any individually identifiable health information created, received, maintained, or transmitted by a covered entity or business associate. PHI includes obvious identifiers (name, address, date of birth, Social Security number) and less obvious ones (medical record numbers, health plan beneficiary numbers, biometric identifiers, photographs).

When PHI exists in electronic form, it is **electronic Protected Health Information (ePHI)**. Most health data today is ePHI, which puts IT systems directly responsible for its storage, transmission, and security.

**De-identified data** is health information stripped of HIPAA's 18 identifiers; HIPAA does not restrict it because it cannot be traced to a specific person. However, research has shown that supposedly de-identified data can sometimes be re-identified by combining it with other sources, raising its own ethical concerns.

### The Privacy Rule

The **HIPAA Privacy Rule** governs who can access PHI and when. Its core principle is the **minimum necessary standard**: covered entities should access, use, or disclose only the minimum PHI needed for a specific purpose. A billing clerk does not need a patient's full medical history to process a claim; a researcher studying treatment outcomes does not need patient names.

The Privacy Rule grants patients specific rights:

* **Right to access:** Patients can request copies of their own records.
* **Right to amendment:** Patients can ask for corrections to inaccurate information.
* **Right to an accounting of disclosures:** Patients can find out who has accessed their records and why.
* **Right to restrict disclosures:** Patients can request limits on how their information is shared.

For IT professionals, the Privacy Rule means system design matters. Access controls, role-based permissions, audit logs, and data segmentation are the mechanisms through which patient rights are protected or violated.

### The Security Rule

Where the Privacy Rule focuses on who can access PHI, the **HIPAA Security Rule** focuses on how ePHI must be protected. It requires three categories of safeguards:

* **Administrative safeguards:** Policies, procedures, and training, including a designated security officer, risk assessments, and staff training.
* **Physical safeguards:** Protecting the infrastructure where ePHI is stored: facility access controls, workstation security, device disposal.
* **Technical safeguards:** Technology-based protections: access controls, audit controls, integrity controls, and transmission security (encryption).

The Security Rule does not prescribe specific technologies; it requires organizations to assess risks and choose "reasonable and appropriate" safeguards. The flexibility lets the rule cover everything from massive hospital systems to two-person clinics, but it also lets organizations treat HIPAA as a checkbox rather than a genuine commitment to patient protection.

### Breach Notification

When PHI is compromised, HIPAA's **Breach Notification Rule** requires covered entities to notify affected individuals, HHS, and (for breaches affecting 500 or more) the media, within 60 days.

Penalties can be severe. Civil fines range from $100 to $50,000 per violation, up to $1.5 million per category annually. Criminal penalties include fines up to $250,000 and prison time for individuals who knowingly obtain or disclose PHI. The HHS Office for Civil Rights maintains a public portal of breaches affecting 500 or more, and the list has grown rapidly as healthcare has become a frequent cyberattack target.

### Think About It 6.1 🧠

> You work as an IT support technician at a small medical clinic. While troubleshooting a printer issue, you see a patient's lab results on a screen. The patient is someone you know personally. HIPAA's minimum necessary standard says you should not have seen that information at all. But you did. What are your ethical obligations at this point? Does it matter whether you tell anyone what you saw?

### Quick Check 6.1 ✅

1. A cloud storage company hosts patient records for a hospital. Is the cloud storage company subject to HIPAA? Explain why or why not. *(Understand)*

2. Explain the difference between the HIPAA Privacy Rule and the HIPAA Security Rule. How do they complement each other? *(Understand)*

3. A medical researcher wants to study treatment outcomes for diabetes patients across five hospitals. The researcher does not need to know patients' names or addresses. Using the concept of the minimum necessary standard, explain how this research could be conducted in a way that respects patient privacy. *(Apply)*

---

## 6.2 Mobile Health and Wireless Technology Ethics

Healthcare is no longer confined to hospitals and clinics. **Mobile health (mHealth)** technology has expanded where and how health data is collected. The convenience brings real benefits and real ethical challenges.

### The mHealth Landscape

mHealth runs from **consumer health apps** (the kind you download to track steps, sleep, or meals) to **regulated medical devices** (continuous glucose monitors, cardiac implants, post-surgery remote monitoring). Regulated devices meet FDA standards and generally fall under HIPAA when connected to a provider's systems. Consumer apps often fall outside both: a fitness tracker recording your heart rate around the clock collects sensitive data, but if it is not connected to a covered entity, HIPAA does not apply, and the app's terms of service govern.

The gap is large. Apps can legally sell aggregated data to insurers, employers, or advertisers; store data on weakly secured servers; or share with third parties, as long as the practice is disclosed somewhere in the terms.

### Wearables and Continuous Monitoring

**Wearable devices**, smartwatches, fitness bands, biosensors, are a rapidly growing category. Modern smartwatches detect irregular heart rhythms, estimate blood oxygen, track menstrual cycles, and identify falls, and have alerted users to atrial fibrillation before symptoms appeared.

Continuous monitoring means continuous data collection. A wearable that tracks location, heart rate, sleep, and activity creates a detailed picture of daily life. Shared with an employer, it could shape job decisions; shared with an insurer, premiums. The question is whether users understand what they have agreed to.

### BYOD in Clinical Settings

**Bring Your Own Device (BYOD)** policies let healthcare workers use personal smartphones and tablets for work: a nurse looking up drug interactions, a physician accessing an EHR from home. BYOD improves efficiency but creates serious security and privacy risks.

Personal devices often lack the encryption, passcode strength, or remote-wipe capability required for ePHI. They connect to unsecured Wi-Fi, are shared with family, and are lost or stolen more easily than organization-issued devices. Each scenario is a potential HIPAA violation.

Organizations balance BYOD productivity against the duty to protect patient data. Some hospitals ban personal devices entirely. Others allow BYOD with mobile device management (MDM) software that controls work-related data on the device. Bans slow care delivery; MDM raises its own privacy concerns, since employees may object to employer control over a personal device.

### Patient Consent for Health Data Collection

Consent is foundational to healthcare ethics and data privacy, but in mHealth it is complicated by the volume of data collected and the difficulty of explaining its possible uses.

A patient agreeing to a doctor-prescribed monitoring device understands the data will go to their care team. But do they understand the manufacturer may also access it, a third-party analytics company may process it, or that de-identified versions may be sold for research? Meaningful consent requires understanding and a genuine choice. Patients often feel they cannot refuse a technology their doctor recommends, and that power imbalance makes consent more ethically charged than in other contexts.

### Case Study 6.1 - Wellness Program Wearables at Midland Manufacturing 📋

**The Situation:** Midland Manufacturing, a company with 2,200 employees, launches a voluntary corporate wellness program in partnership with a wearable device company called VitaTrack. Employees who participate receive a free VitaTrack smartwatch that monitors steps, heart rate, sleep quality, and stress levels. In exchange, participating employees receive a $50 monthly reduction in their health insurance premium.

The program is framed as a benefit. Midland's HR director, Sarah Chen, promotes it at a company meeting: "This is about helping our employees live healthier lives. The data stays with VitaTrack. We only see aggregate reports, never individual data."

Six months into the program, problems surface. Three employees report that their managers have made comments suggesting they know about specific health data. One employee, a warehouse worker named Darnell Washington, is told by his supervisor that he "might want to get more sleep" after a week of low sleep scores. Darnell did not share his sleep data with his supervisor. He files a complaint with HR.

An internal investigation reveals that VitaTrack's "aggregate reports" include department-level breakdowns with groups as small as four people. In a department with only four employees, individual data is effectively identifiable. Additionally, VitaTrack's terms of service, which employees agreed to when activating their watches, allow the company to share "anonymized insights" with Midland's HR department. The terms also permit VitaTrack to use individual health data for "product improvement and research partnerships," which includes selling de-identified data to insurance analytics firms.

**Stakeholders:**

* **Employees who participated** expect their health data to be private and voluntarily joined based on assurances about data separation
* **Midland Manufacturing** wants to reduce healthcare costs and promote employee wellness, but faces liability for the data exposure
* **VitaTrack** profits from both the corporate contract and the secondary data market, and designed the program's data-sharing structure
* **Managers who received department reports** may have acted on health data without realizing they were violating employee privacy
* **Employees who declined to participate** may face implicit pressure to join or may be viewed as less committed to wellness

**Questions to Consider:**

1. Apply the HIPAA framework you learned in Section 6.1 to this scenario. Is the VitaTrack data subject to HIPAA? Why or why not? What does this tell you about the gap between legal compliance and ethical responsibility?

2. Evaluate the consent process in this scenario. Did the employees give meaningful, informed consent to how their data would be used? Consider the concept of power imbalance: can a wellness program offered by your employer ever be truly voluntary?

3. You are an IT professional advising Midland's leadership after the complaint. What changes would you recommend to the program's data practices, and what ethical framework supports each recommendation?

### Quick Check 6.2 ✅

1. Explain the key ethical difference between a consumer fitness app and an FDA-regulated medical device in terms of data protection. *(Understand)*

2. A hospital allows nurses to use personal smartphones to access patient records through a secure app. The hospital requires encryption and a strong passcode on any device used for this purpose. A nurse's phone is stolen from a gym locker. Apply the concept of the minimum necessary standard to evaluate this situation. *(Apply)*

3. A company offers employees a $100 monthly bonus for sharing data from their personal fitness trackers with the company's insurance provider. Analyze the ethical concerns with this arrangement from two stakeholder perspectives: the employee and the insurance provider. *(Analyze)*

---

## 6.3 Clinical IT Systems and Patient Safety

Inside hospitals and clinics, IT systems play a direct role in patient care. When they work, they reduce errors and save lives; when they fail, the consequences fall on patients. Three clinical-IT categories carry the heaviest ethical weight, and telemedicine is rapidly expanding the reach of all three.

### Electronic Health Records (EHRs)

**Electronic Health Records (EHRs)** are digital versions of a patient's medical chart. Unlike paper charts confined to one office, EHRs can be shared across providers, pharmacies, labs, and insurance companies. A primary care physician in Phoenix can see lab results ordered by a specialist in Tucson; an ER doctor treating an unconscious patient can pull a medication list and allergy history.

EHRs reduce duplicate tests, catch dangerous drug interactions, and give providers a more complete picture of a patient's history. The federal government invested heavily through the HITECH Act of 2009, which offered financial incentives for adoption, and most hospitals and physician practices now use EHRs.

Adoption created problems. **Interoperability**, the ability of different EHR systems to exchange data, remains a challenge: a hospital using one vendor may not share records seamlessly with a clinic using another, and patients seeing multiple providers still find records fragmented.

EHRs also create **alert fatigue**. Systems generate so many drug-interaction and allergy alerts that providers override 50% to 90% of them, and the safety system itself becomes a source of risk. IT professionals who design and configure EHRs must keep alerts clinically meaningful, not so frequent they are tuned out.

### Clinical Decision Support Systems (CDSS)

A **Clinical Decision Support System (CDSS)** is software that helps providers make clinical decisions, surfacing evidence-based recommendations: flagging that lab results suggest a condition, recommending a dose based on weight and kidney function, or alerting that a protocol has been updated.

CDSS reduces errors and improves consistency but raises three issues. First, accountability: when CDSS gives a wrong recommendation and the provider follows it, the provider is responsible, but if the software presented inaccurate information, the vendor shares responsibility. Second, the data and rules underneath: a CDSS trained primarily on adult male patients gives less accurate recommendations for women or children. Third, **automation complacency**: heavy reliance erodes independent clinical judgment, and providers may miss what the system does not flag. CDSS supplements clinical expertise; it does not replace it.

### Computerized Provider Order Entry (CPOE)

**Computerized Provider Order Entry (CPOE)** systems let physicians enter medical orders electronically: prescriptions, labs, imaging, and treatment instructions. Before CPOE, illegible handwriting was a documented source of medication errors. CPOE eliminates that and adds safety checks for dosage, interactions, and allergies.

CPOE has reduced some medication errors and introduced new ones: drop-down menus produce wrong selections when drug names look similar, copy-and-paste carries forward outdated information, and documentation time is a persistent source of physician frustration. IT professionals must monitor for unintended consequences and design interfaces that support quality care.

### Telemedicine Ethics

**Telemedicine** delivers healthcare through telecommunications technology. Video consultations, remote monitoring, and digital health platforms expanded dramatically during the COVID-19 pandemic and now let patients in rural areas see distant specialists, reduce travel for elderly and disabled patients, and lower costs.

Telemedicine raises four ethical issues:

* **Access and equity.** It requires reliable internet, a camera-equipped device, and digital literacy. Older adults, low-income patients, and those in rural areas with limited broadband may be excluded from the very technology built to reach them, the **digital divide** in healthcare.

* **Informed consent.** A physician cannot examine a patient through a video call, and some conditions require in-person evaluation. Consent must be specific to the remote format.

* **Privacy and security.** Sessions transmit sensitive health data over the internet. Inadequate encryption or a household where others can overhear compromises patient privacy. The pandemic-era HHS relaxation of HIPAA enforcement for FaceTime and Zoom increased access and increased risk.

* **Cross-state licensing.** Licenses are issued by individual states, so a physician licensed in Arizona generally cannot treat a patient in California without a California license. Telemedicine complicates this; long-term solutions are still developing.

### Think About It 6.3 🧠

> Imagine you are a patient living in a rural community 90 miles from the nearest specialist. Your doctor recommends a telemedicine consultation with a cardiologist. You have a slow internet connection and share your home with family members. What concerns would you have about this arrangement? How would you want the healthcare system to address them?

### Quick Check 6.3 ✅

1. Explain what alert fatigue is and why it represents both a safety problem and an ethical problem in EHR systems. *(Understand)*

2. A small-town physician relies heavily on a CDSS to make prescribing decisions because the clinic cannot afford to hire additional specialists. Analyze the ethical risks and benefits of this level of reliance on a clinical decision support tool. *(Analyze)*

3. A 78-year-old patient with limited internet access is told that her follow-up appointment will be conducted via telemedicine. She has never used a video calling platform. Apply the concept of informed consent to evaluate this situation. What obligations does the healthcare provider have? *(Apply)*

---

## 6.4 AI in Healthcare: Promise, Risk, and Accountability

AI is entering healthcare rapidly. Systems analyze medical images, predict patient deterioration, recommend treatments, accelerate drug discovery, and identify patterns clinicians might miss. The sections that follow build on the Module 3 AI ethics principles, fairness, transparency, accountability, explainability, and human oversight.

### AI-Assisted Diagnostics

Diagnostic AI is among the most visible uses. Systems have detected certain cancers in medical images with accuracy matching or exceeding human radiologists, analyzed retinal scans for diabetic retinopathy, read pathology slides, and identified suspicious skin lesions. They train on labeled image datasets and return probability-based assessments such as "this mammogram has a 94% probability of malignant lesion in a specific quadrant." AI processes images faster than humans, does not tire, and serves as a second set of eyes; in communities with physician shortages, it could extend specialist reach.

But when AI is wrong, the patient bears it. A **false negative** can delay treatment; a **false positive** triggers unnecessary anxiety, testing, and procedures with their own risks.

### Algorithmic Bias in Healthcare AI

**Algorithmic bias** is the tendency of AI systems to perform differently for different populations based on the data they trained on, and it is one of the largest ethical challenges in healthcare AI.

Healthcare AI bias is not hypothetical. A 2019 study (Obermeyer et al.) found that a widely used U.S. hospital algorithm flagging patients for extra care used healthcare spending as a proxy for need. Because Black patients historically had lower spending than white patients with the same illness severity, the algorithm underestimated Black patients' needs; correcting it would have more than doubled the number flagged.

Bias enters at three points:

* **Training data.** If the dataset underrepresents racial, ethnic, age, or gender groups, the system performs less accurately for them.
* **Feature selection.** Zip code can act as a proxy for race or socioeconomic status even when race is not explicitly included.
* **Outcome definitions.** How the algorithm defines "success" or "need" shapes recommendations, as the spending example shows.

Healthcare AI must be tested across diverse populations before deployment, monitored after, and corrected when bias is found. Module 3's fairness and accountability principles apply directly.

### Liability When AI Causes Patient Harm

Medical malpractice frameworks require showing the physician deviated from the standard of care and that the deviation caused harm. AI complicates this. An AI analyzes a chest X-ray and reports no abnormalities; the radiologist, trusting the AI, spends less time reviewing and agrees. Six months later, the patient is diagnosed with lung cancer visible on the original X-ray. Who is responsible?

* **The physician** remains responsible for the final clinical decision. AI is a tool; the physician has a duty of independent judgment.
* **The AI developer** shares responsibility if the system was marketed for a purpose it was not validated for, or if known limitations were not disclosed.
* **The healthcare organization** is responsible for deployment decisions, clinician training, and ongoing performance monitoring.

A deontological view holds the duty of care cannot be delegated to a machine. A utilitarian view asks whether AI-assisted reading, even with errors, produces better aggregate outcomes than human-only reading. Both point to **human oversight**: AI supports clinical decisions; it does not replace the judgment behind them.

### Informed Consent for AI-Assisted Treatment

Should patients be told when AI is involved in their care? The question matters more as AI integrates into diagnostic and treatment workflows.

One side argues patients have a right to know. Informed consent is a cornerstone of medical ethics. If a patient consents to a radiologist reviewing a scan but an algorithm did the analysis, the consent may not cover what happened, and a deontological view treats nondisclosure as a violation of honesty.

The other side argues disclosing every tool is impractical and may cause unnecessary anxiety. Patients are not told which lab machine processed their blood work; AI is just another tool.

No consensus yet. What is clear: **transparency** and **human oversight** point toward giving patients meaningful information about how care decisions get made when AI plays a major role.

### A 2025-2026 Snapshot: Regulation, Ambient Scribes, and Adaptive AI

Two regulatory anchors and one deployment trend define clinical AI ethics in 2025-2026.

**FDA's Predetermined Change Control Plan (PCCP) framework**, finalized in late 2024 / early 2025, lets AI-enabled medical devices update post-market under a pre-authorized plan. It closes a long-standing gap and raises a new question: when a model has changed since deployment, can a clinician still know what they are interpreting?

**The EU AI Act** classifies AI used in healthcare diagnosis or triage as high-risk, with transparency, human-oversight, and post-market monitoring obligations phasing in through 2025-2026.

**Ambient AI scribes** (tools that listen to patient-clinician conversations and draft clinical notes) deployed across U.S. health systems through 2024-2025, raising consent and PHI questions about whether patients know the room is recorded, where audio is processed, and how long it is kept.

Your role is **orchestrator and verifier**: when a clinical AI produces a draft note, triage score, or diagnostic suggestion, ask whether the clinician can see what changed, what the limits are, and what the patient was told.

### Green Computing and Healthcare AI

Training and running AI models takes enormous compute. Large language models and complex imaging algorithms consume energy and rely on hardware with environmental costs. As healthcare adopts more AI, the footprint is an ethical concern.

Per Module 3's green-computing principles, healthcare organizations must weigh environmental impact alongside clinical benefit: efficient models, renewable-powered data centers, and avoiding AI when simpler tools work.

### Think About It 6.4 🧠

> You learn that the AI system your hospital uses to prioritize patients in the emergency department was trained primarily on data from suburban hospitals. Your hospital serves a predominantly low-income, urban community with high rates of chronic disease. What concerns would you raise about this system, and who should you raise them with? Think about the AI ethics principles of fairness and accountability from Module 3.

### Quick Check 6.4 ✅

1. Explain how algorithmic bias can enter a healthcare AI system through training data. Give one specific example of how this might affect patient care. *(Understand)*

2. A hospital begins using an AI tool that reads mammograms and flags potential cancers for radiologist review. The vendor claims the system reduces missed cancers by 20%. Analyze the ethical responsibilities of three parties: the AI developer, the hospital administration, and the radiologist using the system. *(Analyze)*

3. A patient asks you, an IT administrator at a clinic, whether AI is involved in reading their lab results. The clinic's pathology department recently integrated an AI screening tool. Should the patient be told? Apply the ethical principle of transparency to support your answer. *(Apply)*

---

## 6.5 Skills Lab 6A - Ethical Analysis of a Healthcare AI Deployment

**Goal:** Conduct a multi-perspective ethical analysis of a healthcare AI scenario, applying HIPAA principles, stakeholder analysis, and the AI ethics framework from Module 3 to evaluate a real-world deployment decision.

**Estimated time:** 90-120 minutes

### Scenario: AI-Powered Sepsis Prediction at Valley Regional Medical Center

Valley Regional Medical Center (VRMC), a 350-bed community hospital serving a diverse urban population, is considering a contract with a health technology company called MedPredict AI. MedPredict offers an AI-powered sepsis prediction system that monitors patient vital signs, lab results, and EHR data in real time to predict which patients are likely to develop sepsis, a life-threatening response to infection that kills approximately 270,000 Americans each year.

MedPredict's system was developed using data from 12 academic medical centers across the eastern United States. In clinical trials at those institutions, the system identified sepsis an average of six hours before traditional screening methods, with a sensitivity (true positive rate) of 82% and a specificity (true negative rate) of 95%. The company projects that early detection could reduce sepsis mortality at VRMC by up to 15%.

However, VRMC's medical staff has raised several concerns:

* **Population mismatch.** The 12 academic medical centers that provided training data serve a patient population that is predominantly white and privately insured. VRMC's patient population is 45% Hispanic, 20% Black, and 15% uninsured or on Medicaid. Several physicians worry that the system may perform differently for their patients.

* **Alert burden.** With a 95% specificity rate, the system will generate approximately 5 false alerts for every 100 patients screened. VRMC's nurses, who are already managing heavy patient loads, express concern about alert fatigue. They worry that frequent false alarms will lead staff to ignore real alerts.

* **Data integration.** MedPredict's system requires access to real-time EHR data, lab results, and vital signs. This means patient data will flow through MedPredict's cloud servers for processing. MedPredict is a HIPAA-compliant business associate, but some physicians are uncomfortable with the volume of patient data leaving the hospital's network.

* **Cost.** The three-year contract costs $1.8 million. VRMC's administration argues that if the system prevents even a fraction of the sepsis deaths that currently occur, the cost is justified. The chief financial officer notes that sepsis patients who survive often require extended ICU stays costing $50,000 or more per case.

* **Transparency.** MedPredict's algorithm is proprietary. The company provides overall performance statistics but will not share the model's architecture, feature weights, or training methodology. An independent audit of the algorithm is not possible under the proposed contract terms.

### Part 1: Foundation (Aligns with LO1)

1. Identify all stakeholders in this scenario. For each stakeholder, describe their primary interest and what they stand to gain or lose from the deployment decision.

2. Identify which HIPAA provisions are relevant to MedPredict's system. Specifically address: Is MedPredict a covered entity or a business associate? What Security Rule safeguards should VRMC require in the contract? How does the data flow between VRMC and MedPredict's cloud servers affect ePHI protection?

3. Define three key ethical issues raised by this scenario. For each, identify the competing values or rights in tension.

### Part 2: Application (Aligns with LO2)

4. Apply the utilitarian framework to evaluate whether VRMC should deploy MedPredict's system. Identify the potential benefits and harms to each stakeholder group. What does a utilitarian analysis recommend?

5. Apply the deontological framework to evaluate the same decision. Focus specifically on: the duty of care to patients, the transparency concerns around a proprietary algorithm, and the consent implications of routing patient data through an external cloud server.

6. MedPredict's training data underrepresents the demographic groups that make up the majority of VRMC's patient population. Apply the concept of algorithmic bias to explain why this matters. What specific risks does this create, and how should VRMC address them before deploying the system?

### Part 3: Extension (Aligns with LO3)

7. Write a recommendation to VRMC's administration (200-300 words). Should they sign the contract as proposed, negotiate modifications, or decline? Support your recommendation by referencing at least two ethical frameworks and specific concerns from the scenario.

8. Propose three specific contract modifications that would address the ethical concerns you identified. For each modification, explain which ethical principle it protects and why it matters for patient care.

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

## 6.6 Summary and Retrieval 💡

### Key Concepts

* **HIPAA is the legal foundation for U.S. health data privacy.** The Privacy Rule governs PHI access; the Security Rule requires administrative, physical, and technical safeguards for ePHI; the Breach Notification Rule requires disclosure when PHI is compromised.

* **mHealth creates a gap between legal protection and ethical responsibility.** Consumer health apps and wearables often fall outside HIPAA. Meaningful patient consent is hard to achieve when data collection is continuous and downstream uses are opaque.

* **Clinical IT systems improve safety but introduce new risks.** EHRs raise interoperability and alert-fatigue issues. CDSS and CPOE reduce some errors and create others. IT professionals must design and maintain these systems with patient safety as the primary concern.

* **Telemedicine expands access but raises equity, consent, and privacy concerns.** The digital divide can exclude the patients who could benefit most. Consent must cover remote-format limitations. Cross-state licensing remains unresolved.

* **AI in healthcare requires careful ethical oversight.** Algorithmic bias causes disparate performance for underrepresented populations. Liability is shared among developers, organizations, and clinicians. Informed consent, transparency, and human oversight are essential safeguards.

### Key Terms

**Section 6.1**

* **HIPAA:** Federal law setting national standards for health information protection.
* **Protected Health Information (PHI):** Individually identifiable health information held or transmitted by a covered entity or business associate.
* **Electronic PHI (ePHI):** PHI in electronic form.
* **Covered entity:** A healthcare provider, health plan, or healthcare clearinghouse subject to HIPAA.
* **Business associate:** A company handling PHI on behalf of a covered entity; also subject to HIPAA.
* **Privacy Rule:** HIPAA provision governing PHI access, use, and disclosure.
* **Security Rule:** HIPAA provision requiring administrative, physical, and technical safeguards for ePHI.
* **Minimum necessary standard:** Access or disclose only the minimum PHI needed for a specific purpose.
* **Breach Notification Rule:** HIPAA requirement to notify affected individuals and HHS after a PHI breach.

**Section 6.2**

* **mHealth:** Use of mobile devices and wireless tech for healthcare delivery and data collection.
* **BYOD:** Policy allowing employees to use personal devices for work, creating security and privacy challenges.
* **Consumer health app:** A health-related app that may fall outside FDA regulation and HIPAA.

**Section 6.3**

* **Electronic Health Record (EHR):** Digital medical chart shareable across providers and organizations.
* **Interoperability:** The ability of different IT systems to exchange and use data.
* **Alert fatigue:** Clinicians ignoring system-generated alerts due to their high volume.
* **Clinical Decision Support System (CDSS):** Software analyzing patient data and surfacing evidence-based recommendations.
* **Computerized Provider Order Entry (CPOE):** Electronic order entry for prescriptions, labs, imaging, and treatments.
* **Telemedicine:** Remote healthcare delivery via telecommunications technology.
* **Digital divide:** The gap between people with and without access to digital technology, which can widen health disparities.

**Section 6.4**

* **AI-assisted diagnostics:** AI used to analyze medical data and support diagnostic decisions.
* **Algorithmic bias:** AI systems performing differently across populations due to unrepresentative training data or biased features.
* **False negative:** A missed positive (a diseased patient flagged normal).
* **False positive:** A spurious positive (a healthy patient flagged abnormal).
* **Automation complacency:** Reduced independent judgment when humans rely on automated systems.

### Retrieval Practice

Try to answer these from memory before looking back at the module.

1. Name the three categories of safeguards required by the HIPAA Security Rule and give one specific example of each.

2. Explain why a consumer fitness app might collect sensitive health data without being subject to HIPAA. What ethical problem does this gap create for users?

3. A hospital is considering deploying an AI system trained on data from a patient population that does not reflect its own community. Using the concepts from this module, describe two specific risks and two steps the hospital should take before deployment.

---

## 6.7 Discussion Prompt 💬

**Prompt:** During the COVID-19 pandemic, the U.S. Department of Health and Human Services temporarily relaxed HIPAA enforcement for telehealth, allowing providers to use consumer video platforms (such as FaceTime, Zoom, and Skype) that were not fully HIPAA-compliant. The goal was to maintain access to care when in-person visits were not possible. Critics argued this put patient privacy at risk. Supporters argued that denying care to protect privacy was a worse outcome.

Consider this trade-off between access to care and data privacy. To what extent is it ethically justifiable to relax data privacy protections during a public health emergency? In your response, reference at least one ethical framework from this course and consider the perspectives of at least two different stakeholders (for example, a patient in a rural area with limited internet, a healthcare provider, a privacy advocate, or a technology platform). Where should the line be drawn, and who should draw it?

**Guidelines:**

* Your initial post should be 200-300 words
* Reference at least one ethical framework or concept from this module or earlier in the course
* Respond to at least two classmates with substantive engagement

---

## Further Reading 📖

* **U.S. Department of Health and Human Services: "Summary of the HIPAA Privacy Rule."** The official HHS guide to HIPAA's Privacy Rule provisions. Essential reference for understanding patient data protections. Available free at hhs.gov.

* **U.S. Department of Health and Human Services: "Summary of the HIPAA Security Rule."** The official HHS guide to the Security Rule's administrative, physical, and technical safeguard requirements. Available free at hhs.gov.

* **HealthIT.gov: "What Is an Electronic Health Record (EHR)?"** The Office of the National Coordinator for Health Information Technology explains EHR basics, benefits, and challenges. Free government resource.

* **Obermeyer, Z., et al. (2019). "Dissecting Racial Bias in an Algorithm Used to Manage the Health of Populations." *Science*, 366(6464), 447-453.** The landmark study demonstrating algorithmic bias in a healthcare algorithm that systematically underestimated the health needs of Black patients. A foundational reading in healthcare AI ethics.

* **American Medical Association: "Augmented Intelligence in Health Care."** The AMA's policy framework for AI in clinical practice, covering oversight, transparency, and bias mitigation. Available free at ama-assn.org.

---

## Looking Ahead ⏩

In Module 7, you turn from healthcare to software liability and secure coding. When software defects cause harm, who bears responsibility, the developer, the company, or the user? You will examine product-liability frameworks for software, learn secure coding as an ethical obligation, and apply cost/benefit analysis to IT decisions.
