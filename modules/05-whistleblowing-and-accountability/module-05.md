# Module 5: Whistleblowing and Accountability

In October 2021, Frances Haugen, a former data scientist at Facebook (now Meta), appeared before the United States Senate Commerce Committee. She had secretly copied tens of thousands of internal company documents and shared them with journalists and regulators. Those documents revealed that Facebook's own researchers had found evidence that its algorithms amplified misinformation, that Instagram harmed the mental health of teenage users, and that the company had repeatedly chosen growth over safety. Haugen argued that she had tried to raise concerns internally and was ignored. Going public, she said, was the only option left.

Haugen's decision made her a public figure overnight. Supporters called her a hero who put the public interest above corporate loyalty. Critics questioned whether she had the right to take confidential documents and share them with the press. Her case illustrates the core tension at the heart of this module: when does an employee's obligation to the public outweigh their obligation to their employer? And what happens when the information at stake involves the private data of millions of people?

This module examines whistleblowing from both ethical and legal perspectives. You will learn what makes whistleblowing ethically justified, what legal protections exist for whistleblowers, and how fiduciary responsibilities create obligations to protect private information. You will also explore practical guidance for handling a whistleblowing situation, including the emerging role of AI in both enabling and suppressing the act of speaking up.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + activities + discussion)
* **Prerequisites:** Modules 1-4
* **Deliverables:** Discussion post, Quick Checks, Skills Lab analysis
* **CLOs addressed:** CLO V, CLO VII

### Module Learning Objectives *(MLO)* 🎯

By the end of this module, **you will be able to**:

* MLO-5.1 (Understand): **Explain the concept of whistleblowing, distinguish between internal and external whistleblowing, and describe the ethical criteria that justify whistleblowing in IT contexts** *(CLO V)*
* MLO-5.2 (Apply): **Apply legal and ethical frameworks to evaluate whistleblower protections and determine appropriate courses of action in a whistleblowing scenario** *(CLO V)*
* MLO-5.3 (Analyze): **Analyze the fiduciary responsibilities organizations hold regarding private information and examine the ethical tensions between employer loyalty and the duty to protect data subjects** *(CLO VII)*

---

## 5.1 When Is Whistleblowing Ethically Justified?

### Defining Whistleblowing

**Whistleblowing** is the act of reporting illegal, unethical, or harmful activities within an organization to someone who has the power to take corrective action. A **whistleblower** is the person who makes that report. The term carries weight because whistleblowing almost always involves risk. The person reporting the problem is usually an insider, an employee or contractor who has direct knowledge of wrongdoing and chooses to speak up despite the potential consequences.

Whistleblowing is not the same as ordinary workplace complaints. Complaining about a slow coffee machine in the break room is not whistleblowing. Reporting that your company is secretly dumping toxic waste is. The distinction matters because whistleblowing involves exposing conduct that causes serious harm or violates a law, regulation, or ethical standard. It is about accountability at an organizational or societal level, not personal grievances.

In IT, whistleblowing scenarios are common because technology professionals often have access to information that others in the organization do not see. A database administrator might discover that customer data is being sold to third parties without consent. A software engineer might find that a safety-critical system has known bugs that management has decided not to fix. A cybersecurity analyst might learn that the company is concealing a data breach from regulators and affected users. In each case, the IT professional has knowledge that the public or regulators would want to know, and the question becomes: what do you do with it?

### Internal vs. External Whistleblowing

Not all whistleblowing is the same. The first and most important distinction is between **internal whistleblowing** and **external whistleblowing**.

**Internal whistleblowing** means reporting concerns through channels within the organization. You tell your supervisor, the compliance department, the ethics hotline, or the board of directors. The information stays inside the company, and the company has the opportunity to investigate and correct the problem.

**External whistleblowing** means reporting concerns to someone outside the organization: a government regulator, law enforcement, the media, or the public. This is a more dramatic step. It takes the information beyond the organization's control and can result in investigations, lawsuits, public scrutiny, and significant reputational damage.

Most ethical frameworks and legal protections assume that internal reporting should come first. The logic is straightforward: if the organization can fix the problem internally, that is usually the least harmful path. External whistleblowing becomes justified when internal channels fail, when the organization retaliates against the reporter, or when the harm is so immediate and severe that there is no time to wait for an internal response.

### Ethical Criteria for Justified Whistleblowing

Not every disclosure is ethically justified. Leaking confidential information for personal revenge or competitive advantage is not whistleblowing in the ethical sense. Ethical analysis of whistleblowing typically involves several criteria that help distinguish justified disclosure from unauthorized leaking.

**Severity of the harm.** The wrongdoing must involve serious harm, either actual or potential. Exposing a company that is knowingly shipping defective medical devices is different from exposing a company that is merely inefficient. The more serious the potential harm, the stronger the ethical case for speaking up.

**Exhaustion of internal channels.** Before going external, a whistleblower should generally try to resolve the issue internally. If the company has a compliance department, an ethics hotline, or a designated reporting mechanism, using those channels first demonstrates good faith. However, this criterion has limits. If internal channels are controlled by the same people responsible for the wrongdoing, or if using them would put the whistleblower at immediate risk, bypassing them may be justified.

**Reasonable belief in the truth of the claims.** The whistleblower should have a genuine, evidence-based belief that the wrongdoing is occurring. Ethical whistleblowing is based on facts and documentation, not rumors or speculation. This does not mean the whistleblower must have absolute proof, but they should have reasonable grounds for their claims.

**Proportionality.** The act of whistleblowing should be proportionate to the harm being reported. Disclosing more information than necessary to address the wrongdoing, or disclosing information to a wider audience than necessary, raises ethical concerns even when the underlying report is valid.

**Motivation.** While not every ethicist agrees that motivation matters, some frameworks consider it relevant. Is the whistleblower acting out of genuine concern for public safety or justice, or primarily out of personal grievance, financial reward, or revenge? The answer may not change whether the information should be disclosed, but it can affect how the whistleblower's actions are judged.

### Think About It 5.1 🧠

> You discover that your IT department has been storing customer credit card numbers in plain text, a serious security vulnerability that violates industry standards. You report it to your manager, who says, "We know, but fixing it would cost too much and delay our product launch. Keep this to yourself." What would you do next? Which of the ethical criteria above support your decision?

### Quick Check 5.1 ✅

1. In your own words, explain the difference between internal and external whistleblowing. Why do most ethical frameworks recommend trying internal channels first? *(Understand)*

2. A software engineer notices that a colleague is cutting corners on quality testing for a medical device application. The engineer reports it to their manager, who dismisses the concern. Using the ethical criteria from this section, determine whether the engineer would be justified in escalating the report externally. Explain your reasoning. *(Apply)*

3. Why is the criterion of "reasonable belief in the truth of the claims" important for ethical whistleblowing? What risks arise if a person blows the whistle based on rumors rather than evidence? *(Analyze)*

---

## 5.2 Legal Protections for Whistleblowers

Ethical justification is one thing. Legal protection is another. Many people who are ethically justified in blowing the whistle still face devastating personal and professional consequences. Legal protections exist to reduce those consequences, but they are imperfect and inconsistent.

### The Sarbanes-Oxley Act (SOX)

The **Sarbanes-Oxley Act of 2002 (SOX)** was passed after the collapse of Enron and WorldCom, two corporations whose massive accounting fraud destroyed billions of dollars in shareholder value and employee retirement savings. Congress recognized that employees inside these companies had known about the fraud but were afraid to speak up because they feared retaliation.

SOX includes specific whistleblower protections for employees of publicly traded companies. Key provisions include:

* **Protection from retaliation.** Companies cannot fire, demote, suspend, threaten, harass, or discriminate against employees who report suspected fraud to a federal regulatory agency, law enforcement, or a person within the company who has supervisory authority.
* **Complaint process.** Employees who believe they have been retaliated against can file a complaint with the Occupational Safety and Health Administration (OSHA). If OSHA does not act within 180 days, the employee can file a lawsuit in federal court.
* **Criminal penalties.** Individuals who knowingly retaliate against a whistleblower can face fines and up to ten years in prison.

SOX was groundbreaking when it passed, but it has limitations. It applies primarily to employees of publicly traded companies, which means workers at private companies, contractors, and gig workers may not be covered. The complaint process can be slow, and proving retaliation is often difficult because employers can point to other reasons for adverse employment actions.

### The Dodd-Frank Act

The **Dodd-Frank Wall Street Reform and Consumer Protection Act of 2010** expanded whistleblower protections beyond what SOX provided. Passed in response to the 2008 financial crisis, Dodd-Frank added two significant features.

**Financial incentives.** Under Dodd-Frank, whistleblowers who report securities violations to the Securities and Exchange Commission (SEC) can receive between 10% and 30% of monetary sanctions collected as a result of their information, if the sanctions exceed $1 million. Since the program's creation, the SEC has awarded over $2 billion to whistleblowers whose tips led to successful enforcement actions.

**Stronger anti-retaliation provisions.** Dodd-Frank prohibits retaliation against whistleblowers and gives them the right to sue their employer directly in federal court, without first going through OSHA. It also extends protections to a broader range of workers, including some contractors and temporary employees.

The financial incentive structure under Dodd-Frank changed the calculus for potential whistleblowers. Before Dodd-Frank, blowing the whistle was almost entirely a personal sacrifice. The financial rewards do not eliminate the risk, but they do provide some compensation for the career damage and personal stress that whistleblowers often face.

### The False Claims Act

The **False Claims Act (FCA)**, originally passed during the Civil War and significantly amended in 1986, allows private citizens to file lawsuits on behalf of the federal government against entities that have defrauded government programs. This is known as a **qui tam** provision, from the Latin phrase meaning "who sues on behalf of the king."

In IT, the FCA is relevant when companies defraud the government through technology contracts. For example, if a defense contractor bills the government for cybersecurity protections that were never implemented, an employee who discovers the fraud can file a qui tam lawsuit. If the government recovers funds, the whistleblower can receive 15% to 30% of the recovery.

### Limitations of Legal Protections

Despite these laws, whistleblowers continue to face significant risks. Understanding the limitations is essential for anyone considering whether to report wrongdoing.

**Retaliation is hard to prove.** Employers rarely say, "We fired you because you blew the whistle." Instead, they point to performance issues, restructuring, or other seemingly legitimate reasons. Proving that the real reason was retaliation requires evidence that can be difficult to gather.

**Career damage is real and lasting.** Even when whistleblowers win legal cases, many find it difficult to get hired in their industry afterward. Potential employers may view them as disloyal, disruptive, or risky to hire. Research consistently shows that whistleblowers experience higher rates of job loss, financial hardship, and mental health challenges than their peers.

**Coverage gaps exist.** Not all workers are covered by all whistleblower laws. Independent contractors, employees of private companies, and workers in certain industries may have fewer protections. State laws vary widely, creating a patchwork of protections that depends on where you live and who you work for.

**International inconsistency.** Whistleblower protections vary dramatically across countries. The European Union's Whistleblower Protection Directive, adopted in 2019, requires member states to establish internal and external reporting channels and protect whistleblowers from retaliation. Other countries offer little or no protection. For IT professionals working in global organizations, the legal landscape can be confusing and unpredictable.

### Case Study 5.1 - The Quiet Database 📋

**The Situation:** Priya Nair is a senior database administrator at MedVault, a mid-sized health IT company that manages electronic health records for over 200 regional hospitals. During a routine audit, Priya discovers that MedVault's patient data encryption system has a critical flaw: data is encrypted during transmission but stored unencrypted on MedVault's internal servers. This means that anyone with internal server access, including dozens of MedVault employees and contractors, can view unencrypted patient records containing diagnoses, medications, Social Security numbers, and insurance information.

Priya reports the vulnerability to her direct supervisor, Marcus Chen, who escalates it to MedVault's Chief Technology Officer, David Park. Two weeks later, David tells Priya that the company has decided not to fix the vulnerability immediately. The encryption upgrade would cost approximately $2.3 million and require 14 months of development work. MedVault is preparing for a major funding round, and David says the timing is "not right" to disclose a security weakness. He instructs Priya to document the issue but to keep it confidential. "We will get to it after the funding closes," he says.

Three months pass. The funding round is still ongoing, and no action has been taken. Priya learns that MedVault recently signed a contract with a new hospital network, representing the health data of 400,000 additional patients, without disclosing the encryption flaw. She is increasingly concerned that a data breach could expose millions of patient records. She also knows that the Health Insurance Portability and Accountability Act (HIPAA) requires organizations to implement reasonable safeguards for protected health information, and she believes MedVault is in violation.

**Stakeholders:**

* **Priya Nair**, the database administrator who discovered the vulnerability, faces career risk if she escalates externally but feels a professional and ethical obligation to protect patient data
* **Patients** whose health records are stored on MedVault's servers without adequate encryption, including those at the newly signed hospital network who are unaware of the risk
* **MedVault's executives and investors** who are focused on closing a funding round and fear that disclosing the flaw will scare off investors
* **The hospital networks** that contract with MedVault and trust that patient data is being protected according to industry standards and legal requirements
* **Government regulators (HHS Office for Civil Rights)** who enforce HIPAA and have the authority to investigate and penalize organizations that fail to protect health data

**Questions to Consider:**

1. Using the ethical criteria for justified whistleblowing from Section 5.1, evaluate whether Priya would be justified in reporting MedVault's encryption flaw to federal regulators. Consider each criterion (severity, internal channels, reasonable belief, proportionality, motivation) in your analysis.

2. Identify the competing obligations Priya faces. What does she owe to her employer? What does she owe to the patients whose data is at risk? How would a deontological framework from Module 1 help Priya sort through these competing duties?

3. If you were Priya, what would you do at this point? Be specific about the steps you would take and explain the ethical reasoning behind each step.

### Quick Check 5.2 ✅

1. Name the three major federal laws discussed in this section that provide whistleblower protections and briefly describe what each one covers. *(Understand)*

2. A cybersecurity analyst at a private startup discovers that the company is concealing a data breach from customers. The analyst wants to report it but is worried about retaliation. Based on the legal protections discussed in this section, what options does the analyst have, and what limitations might they face? *(Apply)*

3. Why does the financial incentive structure under the Dodd-Frank Act matter ethically? Does paying whistleblowers for information strengthen or weaken the integrity of whistleblowing? Consider arguments on both sides. *(Analyze)*

---

## 5.3 Fiduciary Responsibilities and Private Information

Whistleblowing often involves private information. Sometimes the wrongdoing being reported is the mishandling of that information. To understand the full ethical picture, you need to understand what organizations owe to the people whose data they hold. That obligation is called **fiduciary responsibility**.

### What Is Fiduciary Duty?

A **fiduciary duty** is a legal and ethical obligation to act in the best interest of another party. The concept comes from relationships where one party places trust in another to manage something valuable on their behalf. A doctor has a fiduciary duty to their patient. A lawyer has a fiduciary duty to their client. A financial advisor has a fiduciary duty to the person whose money they manage.

In IT, the concept of fiduciary duty extends to data. When an organization collects personal information from customers, patients, employees, or users, it takes on a responsibility to protect that information. The data does not belong to the organization in the way that inventory or equipment does. It belongs to the individuals it describes, and the organization holds it in trust.

This idea, that data is held in trust rather than owned outright, is the foundation of data privacy law and ethics. It means that organizations have obligations that go beyond simply complying with minimum legal requirements. They have a duty to handle data with care, use it only for purposes the data subjects have agreed to, protect it from unauthorized access, and be transparent about how it is used.

### Data as a Trust

Think of it this way. When you sign up for an online service and provide your name, email address, and phone number, you are not giving that information away. You are lending it to the company for a specific purpose: to create an account, to receive a service, to complete a transaction. The company becomes the **custodian** of that data, and with custodianship comes responsibility.

**Personally identifiable information (PII)** includes any data that can be used to identify a specific individual. Names, addresses, Social Security numbers, phone numbers, email addresses, biometric data, IP addresses, and health records are all examples. The more sensitive the PII, the greater the organization's obligation to protect it.

Organizations that collect PII owe several things to the people whose data they hold:

* **Transparency.** Organizations should clearly explain what data they collect, why they collect it, how they use it, who they share it with, and how long they keep it. Privacy policies should be written in plain language, not buried in pages of legal jargon that no one reads.
* **Purpose limitation.** Data should be used only for the purposes for which it was collected. If a customer provides their email address to receive order confirmations, using that address for marketing without explicit consent violates purpose limitation.
* **Data minimization.** Organizations should collect only the data they actually need. Collecting data "just in case" it might be useful someday is not consistent with fiduciary responsibility.
* **Security.** Organizations must implement reasonable technical and administrative safeguards to protect data from unauthorized access, theft, or accidental exposure.
* **Accountability.** When something goes wrong, the organization must take responsibility. This includes notifying affected individuals, cooperating with regulators, and taking steps to prevent future incidents.

### When Loyalty to Your Employer Conflicts with Duty to Protect Data

This is where fiduciary responsibility connects directly to whistleblowing. An IT professional has an obligation to their employer, but they also have an obligation to the people whose data the employer holds. When those two obligations conflict, the ethical tension can be intense.

Consider this scenario: you work for a company that has experienced a data breach affecting 500,000 customer records. Your employer decides not to disclose the breach to customers or regulators, hoping to fix the vulnerability quietly and avoid bad publicity. You know that affected customers are at risk of identity theft and that several state laws require notification within a specific timeframe.

Your loyalty to your employer pulls you in one direction. Your obligation to the data subjects, the customers whose information was compromised, pulls you in another. Fiduciary responsibility says the obligation to the data subjects should take priority, because the data was entrusted to the organization for safekeeping, and the organization has failed in that duty.

This is not a simple choice. Reporting the breach externally could cost you your job. It could damage the company financially and reputationally. Your coworkers, who had nothing to do with the decision to conceal the breach, could be harmed. But the alternative, staying silent while hundreds of thousands of people remain unaware that their personal information is compromised, carries its own ethical costs.

The ethical frameworks from Module 1 can help sort through this tension. A utilitarian analysis weighs the harm of concealment (potential identity theft for 500,000 people) against the harm of disclosure (financial and reputational damage to the company). A deontological analysis asks whether there is a duty to be honest with the people whose data was compromised, regardless of the consequences. Social contract theory asks what rules a fair society would agree to: would rational people agree to a system where companies can hide data breaches that put them at risk?

### Think About It 5.3 🧠

> You work at a company that sells a popular fitness tracking app. The app collects users' location data, heart rate, sleep patterns, and exercise routines. You discover that the company has been selling aggregated (but not fully anonymized) user health data to insurance companies. The privacy policy technically allows it in a vague clause buried on page 12. Is the company fulfilling its fiduciary duty to users? Does the fact that it is technically "legal" make it ethical? What would you want to know if you were one of the app's users?

### Quick Check 5.3 ✅

1. Define fiduciary duty in your own words and explain how it applies to organizations that collect personal data. *(Understand)*

2. A social media company collects user data for ad targeting and then begins sharing that data with law enforcement agencies without user consent or a court order. Apply the five obligations of data custodianship (transparency, purpose limitation, data minimization, security, accountability) to evaluate whether this practice is ethically defensible. *(Apply)*

3. Analyze the ethical tension between an IT professional's loyalty to their employer and their obligation to protect the data subjects whose information the employer holds. Under what circumstances should the obligation to data subjects take priority? *(Analyze)*

---

## 5.4 Practical Guidance for Handling a Whistleblowing Situation

The first three sections of this module gave you the ethical theory, the legal landscape, and the concept of fiduciary duty. This section turns to practical guidance. If you find yourself in a situation where you believe whistleblowing may be necessary, what should you actually do?

### Step 1: Document Everything

Before you take any action, start collecting evidence. Documentation is the single most important thing a potential whistleblower can do. Without it, your claims may be dismissed as hearsay, and you will have no protection if your employer retaliates.

**What to document:**

* Dates, times, and locations of events you observed
* Names of people involved and their roles
* Copies of relevant emails, messages, reports, or files (be aware of company policies about removing documents, and consult a lawyer before taking proprietary materials)
* Your own written account of what you saw, heard, or discovered, written as close to the event as possible
* Records of any internal reports you made, including who you reported to, when, and what response you received

**Where to keep documentation:** Store copies outside of company systems. A personal email, a secure cloud account, or a physical copy at home are all better than a file on your work laptop that the company can access or delete.

### Step 2: Use Internal Channels First (When Safe to Do So)

As discussed in Section 5.1, starting with internal reporting is usually the right first step, both ethically and legally. Many whistleblower protections require or strongly encourage internal reporting before external disclosure.

Report to your direct supervisor if they are not involved in the wrongdoing. If they are, go to the next level of management, the compliance department, the ethics hotline, or the board of directors. Put your report in writing and keep a copy.

If your organization has a Chief Ethics Officer (as discussed in Module 3), that person is a designated resource for exactly this kind of situation. If the company has a code of ethics, review it. It may outline specific procedures for reporting ethical concerns and describe the protections available to employees who report in good faith.

However, internal reporting is not always safe or effective. You should consider skipping internal channels if:

* The wrongdoing involves senior leadership and there is no independent reporting mechanism
* You have already reported internally and been ignored or told to stay silent
* You have reason to believe that reporting internally will result in the destruction of evidence
* The harm is so immediate and severe that waiting for an internal response would put people at risk

### Step 3: Seek Legal Advice

Before going external, consult a lawyer who specializes in whistleblower cases. This is not optional. The legal landscape is complex, and a single misstep can undermine your protections. A lawyer can help you understand which laws apply to your situation, what evidence you need, how to make a report without exposing yourself to liability, and what financial or legal protections you may be entitled to.

Many whistleblower attorneys offer free initial consultations. Organizations like the Government Accountability Project and the National Whistleblower Center provide resources and referrals.

### Step 4: Report to the Appropriate External Authority

If internal channels have failed or are not an option, the next step is external reporting. The appropriate authority depends on the nature of the wrongdoing:

* **Financial fraud or securities violations:** Securities and Exchange Commission (SEC)
* **Health data violations:** Department of Health and Human Services (HHS), Office for Civil Rights
* **Government contract fraud:** The relevant federal Inspector General, using the False Claims Act
* **Environmental violations:** Environmental Protection Agency (EPA)
* **General workplace safety:** Occupational Safety and Health Administration (OSHA)

Filing a report with the correct agency matters. It activates specific legal protections and ensures that your complaint reaches people with the authority to investigate.

### Step 5: Prepare for the Personal Impact

Whistleblowing is stressful, even when it is the right thing to do. Research consistently shows that whistleblowers face emotional and psychological challenges, including anxiety, isolation, and depression. Professional relationships may suffer. Family members may be affected.

Having a support system matters. This includes legal representation, trusted friends or family, and potentially a therapist or counselor. Some organizations, such as the Whistleblower Network News and ExposeFacts, offer peer support communities for whistleblowers.

### AI Touchpoint: Technology as Both Shield and Weapon

Artificial intelligence is changing the whistleblowing landscape in two important ways, and neither is entirely positive.

**AI-enabled retaliation monitoring.** Some organizations use AI-powered surveillance tools to monitor employee communications, including email, chat, and even keystrokes. These systems can flag "suspicious" behavior, such as searching for information about whistleblower protections, contacting external lawyers, or copying large amounts of data. While companies argue that these tools protect against data theft and insider threats, they can also be used to identify and retaliate against potential whistleblowers before they even make a report. The **accountability** principle from AI ethics (Module 3) raises a critical question here: who is accountable when an AI surveillance system is used to suppress legitimate whistleblowing? If the system flags an employee who is documenting evidence of fraud, and management uses that flag to fire the employee preemptively, both the technology and the people who deployed it bear responsibility.

**AI systems trained on private data.** Many AI systems are trained on datasets that include personal information, sometimes collected without meaningful consent. When a whistleblower discovers that their company's AI models were trained on data that users never agreed to share for that purpose, the situation sits at the intersection of whistleblowing and fiduciary duty. The company has a fiduciary obligation to the data subjects, and the employee who discovers the misuse has a professional obligation to raise the issue. This connects directly to the **transparency** and **fairness** principles from Module 3. If users do not know their data is being used to train AI, the organization is failing its transparency obligation. If the resulting AI system treats certain groups unfairly because of biased or improperly sourced training data, the fairness principle is also violated.

These AI-related scenarios are not hypothetical. Reports from former employees at major technology companies have described exactly these situations: AI surveillance systems used to monitor internal dissent, and AI models trained on data that was collected under one set of promises and used for entirely different purposes.

### Think About It 5.4 🧠

> Imagine you work at a company that uses AI-powered tools to monitor all employee emails and chat messages. You have just discovered evidence that the company is violating customer privacy. You want to report it, but you know the monitoring system might flag your communications with a lawyer or a regulator. How does the existence of AI surveillance change your approach to whistleblowing? What steps would you take to protect yourself?

### Quick Check 5.4 ✅

1. List the five practical steps for handling a whistleblowing situation discussed in this section and briefly explain why each one matters. *(Understand)*

2. An IT security specialist at a private company discovers that customer data is being shared with unauthorized third parties. The specialist has already reported the issue to their manager and the compliance department, but both dismissed the concern. Apply the practical guidance from this section to recommend the specialist's next steps. *(Apply)*

3. How does AI-powered employee surveillance create new ethical challenges for potential whistleblowers? Analyze the tension between a company's legitimate interest in preventing data theft and a whistleblower's need to document and report wrongdoing. *(Analyze)*

---

## 5.5 Skills Lab 5A - The DataStream Dilemma

**Goal:** Analyze a whistleblowing and fiduciary responsibility scenario using ethical criteria, legal frameworks, and AI ethics principles.

**Estimated time:** 90-120 minutes

### Scenario: DataStream Analytics and the Training Data Problem

Kenji Watanabe is a machine learning engineer at DataStream Analytics, a fast-growing company that sells AI-powered customer behavior prediction tools to retailers. DataStream's flagship product, PredictShop, analyzes customer purchase histories, browsing behavior, and location data to predict what products individual customers are likely to buy next. Retailers use PredictShop to personalize marketing, adjust pricing, and manage inventory.

Six months ago, Kenji was assigned to improve PredictShop's accuracy. While reviewing the training data pipeline, he discovered several troubling facts:

* PredictShop is trained on data from a consumer rewards app called ShopPoints, which DataStream acquired two years ago. When ShopPoints users signed up, they agreed to share their data "to improve the ShopPoints experience." The terms of service said nothing about selling data to third parties or using it to train AI models for other companies.
* The training data includes detailed location histories, allowing PredictShop to infer where customers live, work, worship, and receive medical care. None of this information is relevant to predicting purchase behavior, but it remains in the dataset.
* DataStream's retail clients can access individual customer profiles generated by PredictShop, including inferred demographic information such as estimated income level, household composition, and ethnicity. DataStream markets this as a "premium analytics" feature.
* Kenji found that PredictShop's pricing recommendations vary by inferred demographic group, with customers in lower-income zip codes consistently shown higher prices for identical products.

Kenji raised his concerns with his team lead, who told him the data usage was "probably fine" and that the legal team had reviewed the ShopPoints acquisition. Kenji then sent a detailed written report to DataStream's Vice President of Engineering, who responded that the company was "aware of the data sourcing and comfortable with it." No further action was taken.

Kenji now faces a decision. He believes DataStream is violating the trust of millions of ShopPoints users, engaging in discriminatory pricing, and using personal data far beyond what was originally authorized. He is also aware that DataStream recently installed an AI-powered employee monitoring system that flags unusual data access patterns and external communications.

### Part 1: Foundation (Aligns with LO1)

1. Identify all stakeholders in this scenario. For each stakeholder, describe their specific interest and what they stand to gain or lose from Kenji's decision.
2. Using the ethical criteria for justified whistleblowing from Section 5.1, evaluate whether Kenji meets the threshold for ethically justified whistleblowing. Address each criterion (severity, internal channels, reasonable belief, proportionality, motivation).
3. Define fiduciary duty as it applies to this scenario. Explain what DataStream owes to the original ShopPoints users whose data is now being used in ways they did not agree to.

### Part 2: Application (Aligns with LO2)

4. Identify which whistleblower protection laws might apply to Kenji's situation. Explain which law(s) would be most relevant and what limitations he might face. Consider whether DataStream is publicly traded or private and how that affects his options.
5. Apply one ethical framework from Module 1 (utilitarianism, deontology, virtue ethics, or social contract theory) to Kenji's decision. What does your chosen framework recommend he do, and why?

### Part 3: Extension (Aligns with LO3)

6. Analyze the AI ethics dimensions of this scenario. Using the principles from Module 3 (fairness, transparency, accountability, explainability, human oversight), identify which principles DataStream is violating and explain how each violation harms specific stakeholders.
7. Write a 200-300 word recommendation advising Kenji on what to do next. Your recommendation should address the specific steps he should take, the risks he faces (including from the AI monitoring system), and the ethical reasoning that supports your advice.

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

## 5.6 Summary and Retrieval 💡

### Key Concepts

* **Whistleblowing** is the act of reporting illegal, unethical, or harmful activities within an organization. It can be internal (through company channels) or external (to regulators, media, or the public). Ethical whistleblowing is justified when the harm is serious, internal channels have been tried or are ineffective, the whistleblower has a reasonable basis for their claims, and the disclosure is proportionate to the wrongdoing.

* **Legal protections** for whistleblowers include the Sarbanes-Oxley Act (protecting employees of public companies who report fraud), the Dodd-Frank Act (providing financial incentives and stronger anti-retaliation provisions for reporting securities violations), and the False Claims Act (allowing private citizens to sue on behalf of the government for fraud). Despite these protections, whistleblowers continue to face career damage, retaliation that is difficult to prove, and coverage gaps depending on their employment status and location.

* **Fiduciary responsibility** in IT means that organizations holding personal data have an obligation to act in the best interest of the data subjects. This includes transparency about data use, limiting data to its intended purpose, minimizing data collection, implementing strong security, and taking accountability when things go wrong. Data is held in trust, not owned outright, and this distinction carries ethical weight.

* **The tension between employer loyalty and data protection** is one of the defining ethical challenges for IT professionals. When an employer mishandles data, an IT professional's fiduciary obligation to the data subjects may conflict with their loyalty to the organization. Ethical frameworks from Module 1 and the AI ethics principles from Module 3 provide tools for working through this tension.

* **AI creates new challenges for whistleblowers.** AI-powered surveillance tools can be used to identify and suppress potential whistleblowers before they even report. AI systems trained on improperly sourced private data create new categories of wrongdoing that IT professionals may need to report. The principles of accountability and transparency from Module 3 apply directly to both situations.

### Key Terms

**Section 5.1**
* **Whistleblowing:** The act of reporting illegal, unethical, or harmful activities within an organization to someone who can take corrective action.
* **Whistleblower:** A person, usually an insider, who reports organizational wrongdoing.
* **Internal whistleblowing:** Reporting concerns through channels within the organization, such as a supervisor, compliance department, or ethics hotline.
* **External whistleblowing:** Reporting concerns to parties outside the organization, such as regulators, law enforcement, or the media.

**Section 5.2**
* **Sarbanes-Oxley Act (SOX):** A 2002 federal law that includes whistleblower protections for employees of publicly traded companies who report suspected fraud.
* **Dodd-Frank Act:** A 2010 federal law that expanded whistleblower protections, added financial incentives for reporting securities violations, and strengthened anti-retaliation provisions.
* **False Claims Act (FCA):** A federal law that allows private citizens to file lawsuits on behalf of the government against entities that defraud government programs.
* **Qui tam:** A provision of the False Claims Act allowing private citizens to sue on behalf of the government and receive a portion of any recovered funds.

**Section 5.3**
* **Fiduciary duty:** A legal and ethical obligation to act in the best interest of another party, especially when one party has been entrusted with something valuable.
* **Personally identifiable information (PII):** Any data that can be used to identify a specific individual, including names, addresses, Social Security numbers, and biometric data.
* **Data minimization:** The principle that organizations should collect only the personal data they actually need for a stated purpose.
* **Purpose limitation:** The principle that personal data should be used only for the purposes for which it was originally collected.

**Section 5.4**
* **AI-enabled retaliation monitoring:** The use of AI-powered surveillance tools to monitor employee behavior and potentially identify or suppress whistleblowing activity.

### Retrieval Practice

Try to answer these from memory before looking back at the module.

1. Name the four ethical criteria for justified whistleblowing and explain why each one matters.
2. What are the key differences between the whistleblower protections in the Sarbanes-Oxley Act and the Dodd-Frank Act? Which law provides financial incentives, and how does that work?
3. Explain the concept of fiduciary duty as it applies to organizations that hold personal data. Give a specific example of how a company could violate this duty and describe why an IT professional might face a whistleblowing decision as a result.

---

## 5.7 Discussion Prompt 💬

**Prompt:** Frances Haugen's 2021 disclosure of internal Facebook documents sparked a national conversation about whistleblowing in the technology industry. Some praised her for exposing practices that harmed millions of users. Others argued that she violated her employment agreements, disclosed proprietary information, and acted outside proper channels.

Consider this question: When an IT professional discovers that their employer's products are causing widespread harm, do they have an ethical obligation to go public if internal reporting fails? Or does the obligation to respect confidentiality agreements and employer trust take priority?

Take a position and support it using at least one concept from this module (whistleblowing criteria, fiduciary duty, a specific legal protection, or the AI ethics principles from Module 3). Then, address the strongest counterargument to your position. For example, if you argue that whistleblowing is an obligation, explain what limits should exist on that obligation. If you argue that confidentiality should take priority, explain what threshold of harm would change your mind.

**Guidelines:**
* Your initial post should be 200-300 words
* Reference at least one ethical framework or concept from this module
* Respond to at least two classmates with substantive engagement

---

## Further Reading 📖

* **Government Accountability Project: "Whistleblower's Handbook."** A practical guide for employees considering whistleblowing, including information on legal protections, documentation strategies, and support resources. Free online resource at whistleblower.org.

* **SEC Office of the Whistleblower.** The Securities and Exchange Commission's official page on its whistleblower program, including eligibility criteria, how to submit tips, and annual reports on awards paid. Free access at sec.gov/whistleblower.

* **Markkula Center for Applied Ethics: "Whistleblowing."** A concise overview of the ethical considerations surrounding whistleblowing, including analysis of competing obligations and case examples. Free online resource from Santa Clara University.

* **National Whistleblower Center: "Know Your Rights."** A resource covering federal and state whistleblower protection laws, with emphasis on how different laws apply to different industries and types of wrongdoing. Free access at whistleblowers.org.

* **Solove, D.J. and Schwartz, P.M. "Privacy Law Fundamentals."** An accessible introduction to privacy law concepts including fiduciary duty, data protection obligations, and the legal frameworks governing personal information. Available through the college library.

---

## Looking Ahead ⏩

In Module 6, you will shift focus to the ethical challenges of healthcare IT. You will examine how HIPAA establishes the legal framework for protecting health data, how mobile health technologies and telemedicine create new privacy risks, and how clinical IT systems like electronic health records and clinical decision support tools raise questions about patient safety and informed consent. The fiduciary concepts from this module will apply directly, because healthcare organizations hold some of the most sensitive personal data that exists, and the stakes of mishandling it are life and death.
