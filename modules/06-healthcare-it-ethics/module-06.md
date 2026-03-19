# Module 6: Healthcare IT Ethics

In February 2024, a ransomware attack struck Change Healthcare, one of the largest health technology companies in the United States. Change Healthcare processes roughly 15 billion healthcare transactions each year, handling insurance claims, pharmacy operations, and payment systems for hospitals and clinics nationwide. The attack shut down claims processing for weeks. Physicians could not get paid. Pharmacies could not verify insurance coverage. Small medical practices that depended on timely reimbursements faced potential closure. The personal health data of over 100 million Americans was compromised. One cyberattack on one company disrupted healthcare delivery across the entire country.

That incident exposed something important about modern healthcare: it runs on information technology. Electronic health records, mobile health apps, telemedicine platforms, clinical decision support tools, and AI-assisted diagnostics are now woven into how care is delivered, documented, and paid for. Every one of those systems creates ethical questions. Who has access to your health data? What happens when a clinical system gives a wrong recommendation? Is it ethical to use AI to make treatment decisions when the algorithm may perform differently for different populations? These are not theoretical concerns. They are decisions that IT professionals in healthcare settings face every day.

This module examines the ethical challenges that arise when IT meets healthcare. You will learn the legal foundations of health data privacy, evaluate the risks of mobile and wireless technologies in clinical settings, analyze the ethical implications of clinical IT systems and telemedicine, and consider the promise and danger of AI in healthcare. Throughout, you will apply the ethical frameworks from Part I to situations where patient safety, privacy, equity, and innovation pull in different directions.

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

Health data is different from other kinds of personal information. Your browsing history, your shopping preferences, and even your social media posts reveal something about you, but your health records reveal some of the most sensitive details of your life: diagnoses, mental health treatment, prescription medications, genetic test results, reproductive decisions, and substance use history. When that information is exposed, the consequences can include discrimination, social stigma, job loss, and insurance denial.

That sensitivity is why the United States created a specific legal framework for protecting health data. Understanding this framework is the starting point for thinking ethically about healthcare IT.

### The Health Insurance Portability and Accountability Act (HIPAA)

Congress passed the **Health Insurance Portability and Accountability Act (HIPAA)** in 1996. While the law has several purposes, its most significant impact on IT professionals comes from its privacy and security provisions. HIPAA establishes national standards for who can access health data, how it must be protected, and what happens when protection fails.

HIPAA applies to **covered entities**, which include healthcare providers (hospitals, clinics, physicians), health plans (insurance companies, HMOs), and healthcare clearinghouses (organizations that process health data). It also applies to **business associates**, which are companies that handle health data on behalf of covered entities. This is critical for IT professionals because cloud storage providers, software vendors, billing companies, and IT service firms that work with healthcare organizations are all business associates under HIPAA. If you work in IT and your company touches health data in any way, HIPAA applies to you.

### Protected Health Information (PHI)

**Protected Health Information (PHI)** is the core concept in HIPAA's privacy framework. PHI is any individually identifiable health information that is created, received, maintained, or transmitted by a covered entity or business associate. This includes obvious identifiers like a patient's name, address, date of birth, and Social Security number, but it also includes less obvious ones: medical record numbers, health plan beneficiary numbers, biometric identifiers, and even photographs.

When PHI exists in electronic form, it is called **electronic Protected Health Information (ePHI)**. Most health data today is ePHI, which means IT systems are directly responsible for its storage, transmission, and security.

Here is an important distinction: **de-identified data** is health information that has been stripped of all 18 identifiers specified by HIPAA. De-identified data is not subject to HIPAA restrictions because it cannot be traced back to a specific person. However, research has shown that supposedly de-identified data can sometimes be re-identified by combining it with other data sources, which raises its own ethical concerns.

### The Privacy Rule

The **HIPAA Privacy Rule** governs who can access PHI and under what circumstances. The core principle is the **minimum necessary standard**: covered entities should only access, use, or disclose the minimum amount of PHI needed for a specific purpose. A hospital billing clerk does not need to see a patient's full medical history to process an insurance claim. A researcher studying treatment outcomes does not need patient names.

The Privacy Rule grants patients specific rights:

* **Right to access:** Patients can request copies of their own health records.
* **Right to amendment:** Patients can ask for corrections to inaccurate information.
* **Right to an accounting of disclosures:** Patients can find out who has accessed their records and why.
* **Right to restrict disclosures:** Patients can request limits on how their information is shared.

For IT professionals, the Privacy Rule means that system design matters. Access controls, role-based permissions, audit logs, and data segmentation are not just technical features. They are the mechanisms through which patient rights are protected or violated.

### The Security Rule

While the Privacy Rule focuses on who can access PHI, the **HIPAA Security Rule** focuses on how ePHI must be protected. The Security Rule requires covered entities and business associates to implement three categories of safeguards:

* **Administrative safeguards:** Policies, procedures, and training. This includes designating a security officer, conducting risk assessments, and training all staff who handle ePHI.
* **Physical safeguards:** Protecting the physical infrastructure where ePHI is stored. This includes facility access controls, workstation security, and device disposal procedures.
* **Technical safeguards:** Technology-based protections. This includes access controls, audit controls, integrity controls, and transmission security (encryption).

The Security Rule does not prescribe specific technologies. Instead, it requires organizations to assess their risks and choose "reasonable and appropriate" safeguards. This flexibility is intentional because healthcare organizations range from massive hospital systems to two-person clinics, but it also means that some organizations underinvest in security, treating HIPAA compliance as a checkbox exercise rather than a genuine commitment to patient protection.

### Breach Notification

When PHI is compromised, HIPAA's **Breach Notification Rule** requires covered entities to notify affected individuals, the Department of Health and Human Services (HHS), and, for breaches affecting 500 or more individuals, the media. Notifications must occur within 60 days of discovering the breach.

The consequences of a HIPAA violation can be severe. Civil penalties range from $100 to $50,000 per violation, with annual maximums up to $1.5 million per violation category. Criminal penalties can include fines up to $250,000 and prison time for individuals who knowingly obtain or disclose PHI. The HHS Office for Civil Rights maintains a public breach portal listing all breaches affecting 500 or more individuals, and that list has grown significantly in recent years as healthcare organizations become more frequent targets for cyberattacks.

### Think About It 6.1 🧠

> You work as an IT support technician at a small medical clinic. While troubleshooting a printer issue, you see a patient's lab results on a screen. The patient is someone you know personally. HIPAA's minimum necessary standard says you should not have seen that information at all. But you did. What are your ethical obligations at this point? Does it matter whether you tell anyone what you saw?

### Quick Check 6.1 ✅

1. A cloud storage company hosts patient records for a hospital. Is the cloud storage company subject to HIPAA? Explain why or why not. *(Understand)*

2. Explain the difference between the HIPAA Privacy Rule and the HIPAA Security Rule. How do they complement each other? *(Understand)*

3. A medical researcher wants to study treatment outcomes for diabetes patients across five hospitals. The researcher does not need to know patients' names or addresses. Using the concept of the minimum necessary standard, explain how this research could be conducted in a way that respects patient privacy. *(Apply)*

---

## 6.2 Mobile Health and Wireless Technology Ethics

Healthcare is no longer confined to hospitals and clinics. Mobile health technology, commonly called **mHealth**, has expanded where and how health data is collected, shared, and used. Smartphones, wearable fitness trackers, remote patient monitoring devices, and health apps have made it possible to track everything from your heart rate to your blood glucose levels in real time. That convenience brings genuine benefits, but it also creates ethical challenges that the healthcare industry is still working through.

### The mHealth Landscape

The term mHealth covers a broad range of technologies. At one end are **consumer health apps**, the kind you download from an app store to track your steps, monitor your sleep, or log your meals. At the other end are **regulated medical devices**, like continuous glucose monitors, cardiac implantable devices that transmit data to physicians, and remote patient monitoring systems used after surgery.

The distinction matters ethically and legally. Regulated medical devices must meet standards set by the U.S. Food and Drug Administration (FDA) and are generally subject to HIPAA when connected to a healthcare provider's systems. Consumer health apps, however, often fall outside both FDA regulation and HIPAA protection. A fitness tracker that records your heart rate 24 hours a day is collecting sensitive health data, but if it is not connected to a covered entity, HIPAA does not apply. The app's privacy practices are governed by its terms of service, which you may or may not have read.

This gap means that millions of people are generating detailed health data every day with minimal legal protection. The company behind your fitness app might sell aggregated data to insurers, employers, or advertisers. It might store your data on servers with weak security. It might share your data with third parties you have never heard of. All of this can happen legally if it is disclosed somewhere in the terms of service.

### Wearables and Continuous Monitoring

**Wearable devices** like smartwatches, fitness bands, and biosensors represent a rapidly growing category of mHealth. Modern smartwatches can detect irregular heart rhythms, estimate blood oxygen levels, track menstrual cycles, and even identify falls. These features have real health value. There are documented cases of smartwatches alerting users to atrial fibrillation before they experienced symptoms, potentially saving lives.

But continuous monitoring also means continuous data collection. A wearable that tracks your location, heart rate, sleep patterns, and activity levels around the clock creates an extraordinarily detailed picture of your daily life. If that data is shared with an employer, it could be used to make decisions about your job. If shared with an insurance company, it could affect your premiums. The ethical question is whether users truly understand the implications of wearing a device that never stops watching.

### BYOD in Clinical Settings

**Bring Your Own Device (BYOD)** policies allow healthcare workers to use their personal smartphones and tablets for work purposes. A nurse might use a personal phone to look up drug interactions. A physician might use a personal tablet to access a patient's electronic health record from home. BYOD can improve efficiency and convenience, but it creates serious security and privacy risks.

Personal devices may lack the encryption, password protections, or remote-wipe capabilities required for ePHI. They connect to unsecured home Wi-Fi networks and public hotspots. They are shared with family members. They are lost or stolen more easily than organization-issued devices. Each of these scenarios represents a potential HIPAA violation and a breach of patient trust.

The ethical challenge for healthcare organizations is balancing the productivity benefits of BYOD against the duty to protect patient data. Some hospitals have banned personal devices entirely. Others allow BYOD but require mobile device management (MDM) software that gives the organization control over work-related data on the device. Neither approach is perfect. Banning BYOD can slow down care delivery. Requiring MDM raises its own privacy concerns, since healthcare workers may object to their employer having control over their personal device.

### Patient Consent for Health Data Collection

Consent is a foundational principle in both healthcare ethics and data privacy. But in the mHealth space, consent is complicated by the sheer volume of data being collected and the difficulty of explaining what that data might be used for.

When a patient agrees to use a remote monitoring device prescribed by their doctor, they typically understand that their health data will be shared with their care team. But do they understand that the device manufacturer might also access that data? That a third-party analytics company might process it? That de-identified versions of it might be sold for research?

Meaningful consent requires that the person understands what they are agreeing to and has a genuine choice. In healthcare, patients often feel they cannot refuse a technology their doctor recommends, especially if it is presented as part of their treatment. This power imbalance makes the consent process more ethically charged than consent in other technology contexts.

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

Inside hospitals and clinics, IT systems play a direct role in patient care. When these systems work well, they reduce errors, improve coordination, and save lives. When they fail or are poorly designed, the consequences fall on patients. This section examines three major categories of clinical IT and the ethical obligations they create, then looks at how telemedicine is expanding the reach of healthcare while raising new ethical questions.

### Electronic Health Records (EHRs)

**Electronic Health Records (EHRs)** are digital versions of a patient's medical chart. Unlike paper charts that stayed in one office, EHRs can be shared across providers, pharmacies, labs, and insurance companies. A primary care physician in Phoenix can see the results of a blood test ordered by a specialist in Tucson. An emergency room doctor treating an unconscious patient can access their medication list and allergy information.

The potential benefits are significant. EHRs reduce duplicate tests, catch dangerous drug interactions, and give providers a more complete picture of a patient's health history. The federal government recognized this potential and invested heavily through the HITECH Act of 2009, which offered financial incentives to healthcare providers who adopted EHR systems. Today, the vast majority of hospitals and physician practices use EHRs.

But EHR adoption has also created problems. **Interoperability**, the ability of different EHR systems to exchange data, remains a major challenge. A hospital using one EHR vendor may not be able to share records seamlessly with a clinic using a different vendor. This means that the promise of a complete, portable medical record has not been fully realized. Patients who see multiple providers may still find that their records are fragmented, leading to repeated tests, missed information, and potential safety gaps.

EHRs also create ethical concerns around **alert fatigue**. EHR systems generate automated alerts for drug interactions, allergy warnings, and other clinical issues. In theory, these alerts prevent errors. In practice, providers receive so many alerts that they begin ignoring them. Studies have found that clinicians override 50% to 90% of EHR alerts. When providers routinely dismiss warnings, the system designed to improve safety becomes a source of risk. IT professionals who design, configure, and maintain EHR systems have an ethical responsibility to ensure that alerts are clinically relevant and not so frequent that they lose their effectiveness.

### Clinical Decision Support Systems (CDSS)

A **Clinical Decision Support System (CDSS)** is software that helps healthcare providers make clinical decisions. CDSS tools analyze patient data and provide evidence-based recommendations. For example, a CDSS might flag that a patient's lab results suggest a specific condition, recommend a particular medication dosage based on the patient's weight and kidney function, or alert a provider that a treatment protocol should be adjusted based on new clinical guidelines.

CDSS can reduce medical errors and improve the consistency of care. But these systems also raise important ethical questions. First, who is responsible when a CDSS gives a wrong recommendation and a provider follows it? The provider is still legally and ethically responsible for the treatment decision, but if the software presented inaccurate information, the software vendor may share some responsibility. The lines of accountability are not always clear.

Second, CDSS systems are only as good as the data and rules they are built on. If the underlying clinical evidence is incomplete, outdated, or biased toward certain populations, the recommendations will reflect those gaps. A CDSS trained primarily on data from adult male patients, for example, might give less accurate recommendations for women or children.

Third, there is the risk of **automation complacency**. When providers rely heavily on a CDSS, they may reduce their own independent clinical judgment. If the system becomes a crutch rather than a tool, providers may miss things the system does not flag. The ethical obligation is to use CDSS as a supplement to clinical expertise, not a replacement for it.

### Computerized Provider Order Entry (CPOE)

**Computerized Provider Order Entry (CPOE)** systems allow physicians to enter medical orders electronically: prescriptions, lab tests, imaging studies, and treatment instructions. Before CPOE, these orders were handwritten, and illegible handwriting was a well-documented source of medication errors. CPOE systems eliminate that problem and add safety checks, such as verifying dosages, checking for drug interactions, and flagging allergies.

CPOE has measurably reduced certain types of medication errors. However, the systems have also introduced new types of errors. Drop-down menus can lead to wrong selections when drug names look similar. Copy-and-paste functions can carry forward outdated or incorrect information from previous orders. And the time required to enter orders electronically has been a consistent source of frustration for physicians, who report spending more time on documentation and less time with patients.

The ethical dimension is this: CPOE systems were adopted primarily to improve patient safety, and they have succeeded in some areas. But when the same systems create new error pathways and reduce face-to-face patient interaction, the net benefit is not as straightforward as it first appears. IT professionals who build and maintain these systems have an obligation to monitor for unintended consequences and design interfaces that support, rather than hinder, quality care.

### Telemedicine Ethics

**Telemedicine** uses telecommunications technology to deliver healthcare remotely. Video consultations, remote patient monitoring, and digital health platforms expanded dramatically during the COVID-19 pandemic, when in-person visits became difficult or impossible. Telemedicine allows patients in rural areas to see specialists hundreds of miles away. It reduces travel time for elderly and disabled patients. It can lower costs for both patients and providers.

But telemedicine also raises ethical questions that the healthcare system is still working through:

* **Access and equity.** Telemedicine requires a reliable internet connection, a device with a camera, and a level of digital literacy that not all patients have. Older adults, low-income patients, and those in rural areas with limited broadband access may be excluded from the very technology designed to reach them. This is the **digital divide** applied to healthcare, and it means that telemedicine can widen health disparities even as it closes geographic ones.

* **Informed consent.** Patients using telemedicine should understand the limitations of a remote visit. A physician cannot perform a physical examination through a video call. Certain conditions require in-person evaluation. Patients need to know what telemedicine can and cannot do, and they need to consent specifically to the remote format.

* **Privacy and security.** Telemedicine sessions transmit sensitive health information over the internet. If the platform is not properly encrypted, or if the patient is in a location where others can overhear the conversation, patient privacy is compromised. During the pandemic, HHS temporarily relaxed HIPAA enforcement for telehealth, allowing providers to use platforms like FaceTime and Zoom that were not fully HIPAA-compliant. While that flexibility increased access, it also increased risk.

* **Cross-state licensing.** In the United States, medical licenses are issued by individual states. A physician licensed in Arizona cannot typically treat a patient located in California without a California license. Telemedicine complicates this because the patient and provider can be anywhere. Some states created temporary interstate practice agreements during the pandemic, but long-term solutions are still being developed. The ethical tension is between expanding patient access and maintaining the regulatory oversight that licensing provides.

### Think About It 6.3 🧠

> Imagine you are a patient living in a rural community 90 miles from the nearest specialist. Your doctor recommends a telemedicine consultation with a cardiologist. You have a slow internet connection and share your home with family members. What concerns would you have about this arrangement? How would you want the healthcare system to address them?

### Quick Check 6.3 ✅

1. Explain what alert fatigue is and why it represents both a safety problem and an ethical problem in EHR systems. *(Understand)*

2. A small-town physician relies heavily on a CDSS to make prescribing decisions because the clinic cannot afford to hire additional specialists. Analyze the ethical risks and benefits of this level of reliance on a clinical decision support tool. *(Analyze)*

3. A 78-year-old patient with limited internet access is told that her follow-up appointment will be conducted via telemedicine. She has never used a video calling platform. Apply the concept of informed consent to evaluate this situation. What obligations does the healthcare provider have? *(Apply)*

---

## 6.4 AI in Healthcare: Promise, Risk, and Accountability

Artificial intelligence is entering healthcare at a rapid pace. AI systems can analyze medical images, predict patient deterioration, recommend treatment options, accelerate drug discovery, and identify patterns in health data that human clinicians might miss. The potential to improve care and save lives is real. But so are the risks. This section examines the ethical dimensions of AI in healthcare, building on the AI ethics principles you studied in Module 3: fairness, transparency, accountability, explainability, and human oversight.

### AI-Assisted Diagnostics

Some of the most visible uses of AI in healthcare involve diagnostics. AI systems have demonstrated the ability to detect certain cancers in medical images with accuracy that matches or exceeds human radiologists. Algorithms can analyze retinal scans for signs of diabetic retinopathy, read pathology slides for evidence of cancer, and identify skin lesions that may be melanoma.

These systems work by training on large datasets of labeled medical images. The algorithm learns to associate visual patterns with specific diagnoses. When presented with a new image, it provides a probability-based assessment. A system might report that a mammogram has a 94% probability of showing a malignant lesion in a specific quadrant.

The benefits are compelling. AI can process images faster than humans, never gets tired, and can serve as a second set of eyes that catches what a busy radiologist might miss. In areas with physician shortages, AI diagnostics could extend the reach of specialists to underserved communities.

But there are critical ethical questions. What happens when the AI is wrong? A **false negative**, where the system says a scan is normal when it is not, can delay treatment and allow a disease to progress. A **false positive**, where the system flags something that turns out to be benign, can cause unnecessary anxiety, additional testing, and medical procedures with their own risks. In both cases, the patient bears the consequence.

### Algorithmic Bias in Healthcare AI

One of the most significant ethical challenges in healthcare AI is **algorithmic bias**: the tendency of AI systems to perform differently for different populations based on the data they were trained on.

Healthcare AI bias is not hypothetical. A widely reported 2019 study examined an algorithm used by hospitals across the United States to identify patients who would benefit from additional care. The algorithm used healthcare spending as a proxy for healthcare needs. Because of systemic inequities, Black patients historically had lower healthcare spending than white patients with the same level of illness. The result was that the algorithm systematically underestimated the health needs of Black patients. The researchers found that correcting this bias would have more than doubled the number of Black patients identified for additional care.

Bias can enter healthcare AI at multiple points:

* **Training data.** If the dataset used to train an AI system underrepresents certain racial, ethnic, age, or gender groups, the system will perform less accurately for those groups. Most clinical research data has historically overrepresented white male patients, which means AI systems trained on that data may be less effective for women, people of color, and older adults.

* **Feature selection.** The choice of which variables to include in an algorithm can introduce bias. Using zip code as a feature, for example, can function as a proxy for race or socioeconomic status, even if race is not explicitly included.

* **Outcome definitions.** How the algorithm defines "success" or "need" shapes its recommendations. The healthcare spending example above shows how a seemingly neutral metric can embed existing inequities.

The ethical obligation is clear: AI systems in healthcare must be tested across diverse populations before deployment, monitored for disparate performance after deployment, and corrected when bias is found. The AI ethics principles from Module 3, especially fairness and accountability, are directly applicable here.

### Liability When AI Causes Patient Harm

When a physician makes a diagnostic error, there are well-established legal frameworks for determining responsibility. Medical malpractice law requires the patient to show that the physician deviated from the standard of care and that the deviation caused harm. But when an AI system contributes to a diagnostic error, the question of liability becomes more complicated.

Consider this scenario: An AI system analyzes a chest X-ray and reports no abnormalities. The radiologist, trusting the AI's assessment, spends less time reviewing the image and agrees with the AI's conclusion. Six months later, the patient is diagnosed with lung cancer that was visible on the original X-ray. Who is responsible?

There are several possible answers, and legal frameworks are still developing:

* **The physician** remains responsible for the final clinical decision. AI is a tool, and the physician has a duty to exercise independent judgment.
* **The AI developer** may bear some responsibility if the system was marketed for a purpose it was not validated for, or if known limitations were not disclosed.
* **The healthcare organization** may be responsible for how it deployed the AI system, whether it provided adequate training to clinicians, and whether it monitored the system's performance.

From a deontological perspective, the physician has a duty of care to the patient that cannot be delegated to a machine. From a utilitarian perspective, the question is whether AI-assisted reading, even with its errors, produces better overall outcomes than human-only reading. Both perspectives point to the importance of **human oversight**: AI should support clinical decisions, not replace the human judgment behind them.

### Informed Consent for AI-Assisted Treatment

Should patients know when AI is involved in their care? This question is increasingly relevant as AI systems are integrated into diagnostic and treatment workflows.

Some argue that patients have a right to know. Informed consent is a cornerstone of medical ethics. If a patient consents to a radiologist reviewing their scan, but the actual analysis was performed by an algorithm, the patient's consent may not cover what actually happened. From a deontological perspective, failing to disclose AI involvement in care could violate the duty of honesty and transparency.

Others argue that disclosing every tool used in care delivery is impractical and could cause unnecessary anxiety. Patients are not told which specific laboratory machine processed their blood work or which version of a software system generated their MRI images. AI, from this perspective, is just another clinical tool.

There is no consensus yet, and practices vary widely. What is clear is that the ethical principles of **transparency** and **human oversight** both point toward giving patients meaningful information about how their care decisions are made, especially when AI plays a significant role.

### Green Computing and Healthcare AI

Training and running AI models requires enormous computational resources. Large language models and complex imaging algorithms consume significant energy, generate heat that must be cooled, and rely on hardware with environmental costs. As healthcare systems adopt more AI tools, the environmental footprint of that technology is an emerging ethical concern.

This connects to the green computing concepts discussed in Module 3. Healthcare organizations that adopt AI have an ethical responsibility to consider the environmental impact alongside the clinical benefit. Choosing more efficient models, using renewable energy for data centers, and avoiding unnecessary AI deployment when simpler tools would work are all part of that responsibility.

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

### Rubric - Skills Lab 6A

| Criteria | Mastery (5) | Proficiency (4) | Developing (3) | Emerging (2) | Not Evident (1) |
|---|---|---|---|---|---|
| **Stakeholder and HIPAA Analysis** | Identifies all major stakeholders with specific interests; accurately applies HIPAA concepts including business associate status, Security Rule safeguards, and ePHI protections | Identifies most stakeholders with reasonable descriptions; applies HIPAA concepts correctly with minor gaps | Identifies some stakeholders; applies HIPAA concepts with gaps or limited specificity | Lists stakeholders without meaningful description; HIPAA references are vague or inaccurate | Missing or inaccurate stakeholder identification; no HIPAA application |
| **Ethical Framework Application** | Applies utilitarian and deontological frameworks accurately with clear reasoning tied to specific scenario details; demonstrates understanding of each framework's logic | Applies both frameworks correctly with adequate reasoning and some scenario-specific detail | Applies frameworks but with gaps in reasoning or loose connection to the scenario | Attempts to apply frameworks but with significant errors or confusion between them | No ethical framework applied or framework is unrecognizable |
| **Algorithmic Bias Analysis** | Thoroughly explains how training data bias affects performance for VRMC's patient population; identifies specific risks and proposes evidence-based mitigation strategies | Explains training data bias with adequate specificity; identifies risks and proposes reasonable mitigation | Mentions bias but lacks specificity about how it affects this population; mitigation is vague | Acknowledges bias exists but does not connect it to the scenario's demographics | No discussion of algorithmic bias |
| **Recommendation Quality** | Recommendation is clear, specific, and supported by multiple ethical frameworks with explicit reasoning; contract modifications are practical and directly address identified concerns | Recommendation is clear and supported by at least one framework; modifications are reasonable | Recommendation is present but weakly supported; modifications are vague or not clearly connected to concerns | Recommendation is vague or unsupported; modifications are missing or impractical | No recommendation provided |
| **Writing and Professionalism** | Writing is clear, well-organized, and uses healthcare IT and ethical terminology accurately throughout; ideas flow logically between sections | Writing is clear with mostly accurate terminology; organization is generally logical | Writing is understandable but disorganized or imprecise in terminology use | Writing is unclear, contains frequent errors, or lacks professional tone | Unreadable or off-topic |

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.
* **Due:** See Canvas calendar for deadline

---

## 6.6 Summary and Retrieval 💡

### Key Concepts

* **HIPAA provides the legal foundation for health data privacy** in the United States. The Privacy Rule governs who can access PHI. The Security Rule governs how ePHI must be protected. The Breach Notification Rule requires disclosure when PHI is compromised. Together, they create a framework that IT professionals in healthcare must understand and implement.

* **Mobile health technologies create a gap between legal protection and ethical responsibility.** Consumer health apps and wearables often fall outside HIPAA's reach, even though they collect sensitive health data. Meaningful patient consent is difficult to achieve when data collection is continuous and the implications are complex.

* **Clinical IT systems improve patient safety but also introduce new risks.** EHRs improve data access and coordination but suffer from interoperability challenges and alert fatigue. CDSS and CPOE systems reduce certain errors while creating new ones. IT professionals have an ethical responsibility to design, monitor, and maintain these systems with patient safety as the primary concern.

* **Telemedicine expands access but raises equity, consent, and privacy concerns.** The digital divide means that patients who could benefit most from remote care may lack the technology to use it. Consent for telemedicine must address the limitations of remote evaluation. Cross-state licensing creates regulatory complications that are still being resolved.

* **AI in healthcare holds enormous promise but demands careful ethical oversight.** Algorithmic bias can cause AI systems to perform less accurately for underrepresented populations. Liability for AI-related harm is shared among developers, healthcare organizations, and clinicians. Informed consent, transparency, and human oversight are essential safeguards.

### Key Terms

**Section 6.1**

* **HIPAA (Health Insurance Portability and Accountability Act):** Federal law establishing national standards for the protection of health information.
* **Protected Health Information (PHI):** Individually identifiable health information created, received, maintained, or transmitted by a covered entity or business associate.
* **Electronic Protected Health Information (ePHI):** PHI that exists in electronic form.
* **Covered entity:** A healthcare provider, health plan, or healthcare clearinghouse subject to HIPAA.
* **Business associate:** A company that handles PHI on behalf of a covered entity, also subject to HIPAA.
* **Privacy Rule:** HIPAA provision governing who can access, use, and disclose PHI.
* **Security Rule:** HIPAA provision requiring administrative, physical, and technical safeguards to protect ePHI.
* **Minimum necessary standard:** The principle that only the minimum amount of PHI needed for a specific purpose should be accessed or disclosed.
* **Breach Notification Rule:** HIPAA requirement that covered entities notify affected individuals and HHS when PHI is compromised.

**Section 6.2**

* **mHealth (mobile health):** The use of mobile devices and wireless technologies to support healthcare delivery and health data collection.
* **BYOD (Bring Your Own Device):** A policy allowing employees to use personal devices for work purposes, creating security and privacy challenges in healthcare.
* **Consumer health app:** A health-related application that may not be subject to FDA regulation or HIPAA protection.

**Section 6.3**

* **Electronic Health Record (EHR):** A digital version of a patient's medical chart that can be shared across providers and healthcare organizations.
* **Interoperability:** The ability of different IT systems to exchange and use data, a persistent challenge in healthcare IT.
* **Alert fatigue:** The tendency for clinicians to ignore or override system-generated alerts due to their high volume, reducing the safety benefit of the alert system.
* **Clinical Decision Support System (CDSS):** Software that analyzes patient data and provides evidence-based clinical recommendations to healthcare providers.
* **Computerized Provider Order Entry (CPOE):** A system allowing physicians to enter medical orders electronically, reducing handwriting errors while introducing new workflow challenges.
* **Telemedicine:** The use of telecommunications technology to deliver healthcare services remotely.
* **Digital divide:** The gap between populations with access to digital technology and those without, which in healthcare can widen rather than narrow health disparities.

**Section 6.4**

* **AI-assisted diagnostics:** The use of artificial intelligence to analyze medical data (images, lab results, patient records) and support diagnostic decisions.
* **Algorithmic bias:** The tendency of AI systems to perform differently for different populations based on unrepresentative training data or biased feature selection.
* **False negative:** An AI or test result that incorrectly indicates the absence of a condition, potentially delaying treatment.
* **False positive:** An AI or test result that incorrectly indicates the presence of a condition, potentially causing unnecessary intervention.
* **Automation complacency:** The tendency of human professionals to reduce independent judgment when relying on automated systems, increasing the risk of missed errors.

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

In Module 7, you will shift from the healthcare environment to the broader question of software liability and secure coding. When software defects cause harm, who bears responsibility: the developer, the company, or the user? You will examine product liability frameworks applied to software, learn about secure coding principles as an ethical obligation, and apply cost/benefit analysis to IT decision-making, building directly on the risk-assessment thinking you practiced in this module.
