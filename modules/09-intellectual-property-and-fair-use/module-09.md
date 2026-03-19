# Module 9: Intellectual Property and Fair Use

In January 2023, three visual artists filed a class-action lawsuit against Stability AI, Midjourney, and DeviantArt, claiming that these companies trained their AI image generators on billions of copyrighted images scraped from the internet without permission or compensation. The artists argued that every AI-generated image was, in some sense, a derivative of their stolen work. The companies countered that training AI on publicly available data is transformative and falls within the bounds of fair use. As of early 2026, the case remains one of several high-profile lawsuits reshaping how we think about ownership in the age of generative AI. Who is right? The answer depends on how you interpret intellectual property law, and the law is still catching up to the technology.

This module examines the legal and ethical foundations of **intellectual property (IP)**, the body of law that protects creative and innovative works. You will learn the four main types of IP protection, how **fair use** works (and where it falls short in digital contexts), and why open source licensing represents a fundamentally different philosophy about ownership. You will also confront some of the hardest questions in IT ethics right now: Is downloading a movie without paying for it really "theft"? Can a company reverse-engineer a competitor's product legally? And who, if anyone, owns the output of an AI system?

These are not abstract questions. Whether you work in software development, IT support, web design, or data analytics, you will encounter IP decisions regularly. Understanding the rules, and knowing where the rules are genuinely unclear, will help you make informed choices in your career.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + activities + discussion)
* **Prerequisites:** Modules 1-8
* **Deliverables:** Discussion post, Quick Checks, Skills Lab analysis
* **CLOs addressed:** CLO XI

### Module Learning Objectives *(MLO)* 🎯

By the end of this module, **you will be able to**:

* MLO-9.1 (Apply): **Apply the principles of copyright, patent, trademark, and trade secret law to classify real-world IP scenarios** *(CLO XI)*
* MLO-9.2 (Analyze): **Analyze how fair use doctrine applies to digital content, open source licensing, and competitive intelligence practices** *(CLO XI)*
* MLO-9.3 (Evaluate): **Evaluate the ethical and legal arguments surrounding AI-generated works and the use of copyrighted training data** *(CLO XI)*

---

## 9.1 The Four Types of Intellectual Property

Intellectual property is a legal concept that grants creators and inventors certain exclusive rights over their work. Unlike physical property, IP protects intangible things: ideas expressed in a particular form, inventions, brand identities, and confidential business information. The goal of IP law is to reward creativity and innovation while still allowing the public to benefit from new ideas over time.

There are four main types of IP protection, each designed for a different kind of work. Understanding the differences matters because using the wrong framework, or ignoring these protections entirely, can have serious legal and ethical consequences.

### Copyright

**Copyright** protects original works of authorship that are fixed in a tangible form. This includes books, music, software code, photographs, videos, website content, and architectural designs. Copyright protection is automatic: the moment you write a poem, take a photograph, or commit code to a repository, you own the copyright. You do not need to register it, though registration provides additional legal benefits if you ever need to enforce your rights in court.

Copyright gives the owner several exclusive rights: the right to reproduce the work, distribute copies, create derivative works (such as translations or adaptations), and publicly display or perform it. These rights last for a long time. For works created by individuals, copyright protection lasts for the author's lifetime plus 70 years. For works created as **work for hire** (such as software written by an employee as part of their job), the copyright belongs to the employer, and protection lasts 95 years from publication or 120 years from creation, whichever is shorter.

One critical point for IT professionals: **copyright protects the expression of an idea, not the idea itself.** You can write your own sorting algorithm, but you cannot copy someone else's specific code that implements one. Two people can independently write programs that do the same thing, and both programs are separately copyrightable. The protection covers the particular way the idea was expressed in code.

### Patents

A **patent** gives an inventor the exclusive right to make, use, and sell an invention for a limited time, typically 20 years from the filing date. Unlike copyright, patents require a formal application process through the United States Patent and Trademark Office (USPTO) or equivalent agencies in other countries. The invention must be novel, non-obvious, and useful.

In IT, patents cover hardware inventions, manufacturing processes, and sometimes software-related innovations. **Software patents** have been controversial for decades. Critics argue that many software patents are too broad or too obvious, and that they stifle innovation rather than encourage it. A single smartphone may involve thousands of patents held by dozens of companies. Patent disputes in the tech industry have led to massive lawsuits and complex licensing agreements. In 2012, Apple and Samsung fought a patent case over smartphone design elements that eventually reached the U.S. Supreme Court.

### Trademarks

A **trademark** protects words, phrases, symbols, logos, or designs that identify the source of goods or services. The Apple logo, the Nike swoosh, and the phrase "Just Do It" are all trademarks. Trademarks prevent consumer confusion by ensuring that when you see a particular brand name or logo, you know who made the product.

Trademark protection can last indefinitely, as long as the mark is actively used in commerce and the owner takes steps to defend it. This is different from copyright and patents, which eventually expire. For IT professionals, trademarks matter in web development, app design, domain name registration, and anywhere brand identity intersects with technology.

### Trade Secrets

A **trade secret** is confidential business information that provides a competitive advantage. The classic example is the Coca-Cola formula, but in IT, trade secrets more commonly include proprietary algorithms, customer databases, pricing strategies, and internal business processes. Unlike patents, trade secrets have no expiration date and require no registration. The catch is that the owner must take reasonable steps to keep the information secret. If a trade secret is publicly disclosed, whether through a leak, reverse engineering, or carelessness, the protection is lost.

The **Defend Trade Secrets Act (DTSA)** of 2016 created a federal cause of action for trade secret theft, giving companies a powerful legal tool to pursue employees or competitors who misappropriate confidential information. For IT workers, this is especially relevant: the code you write, the systems you build, and the data you access at work may all be classified as trade secrets by your employer.

### Think About It 9.1 🧠

> You create a mobile app on your own time using your own equipment. Your employer claims it belongs to them because it is related to the company's business. What type of IP protection is most relevant here, and who do you think should own the app? What facts would you need to know to decide?

### Quick Check 9.1 ✅

1. What is the key difference between copyright and patent protection? Give an example of something protected by each. *(Understand)*
2. A software company keeps its recommendation algorithm confidential and requires all employees to sign nondisclosure agreements. What type of IP protection applies, and what could cause the company to lose that protection? *(Apply)*
3. Explain why copyright protects the expression of an idea but not the idea itself. Why does this distinction matter for software developers? *(Analyze)*

---

## 9.2 Fair Use, Open Source, and Digital Licensing

Understanding IP types is only half the picture. Equally important is understanding when and how others can legally use protected works. This section covers three frameworks that define the boundaries of legitimate use: fair use doctrine, open source licensing, and the broader ethics of digital content sharing.

### Fair Use Doctrine

**Fair use** is a legal doctrine built into U.S. copyright law (Section 107 of the Copyright Act) that allows limited use of copyrighted material without permission from the copyright holder. Fair use exists because rigid copyright enforcement could stifle criticism, education, commentary, and creativity. A book reviewer needs to quote passages. A teacher needs to share excerpts with students. A comedian needs to parody a popular song. Fair use makes these activities possible.

Courts evaluate fair use claims using four factors:

1. **The purpose and character of the use.** Is the use commercial or nonprofit/educational? Is it "transformative," meaning it adds new meaning, expression, or purpose to the original? Transformative uses are more likely to qualify as fair use.
2. **The nature of the copyrighted work.** Using factual works (like news articles) is more likely to be considered fair use than using highly creative works (like novels or music).
3. **The amount used.** Using a small portion of a work is more defensible than using the entire thing. However, even a small amount can fail the fair use test if it represents the "heart" of the original work.
4. **The effect on the market.** Does the use substitute for the original, potentially reducing sales or licensing revenue? If so, it is less likely to qualify as fair use.

No single factor is decisive. Courts weigh all four together, which makes fair use inherently unpredictable. This ambiguity is one of the biggest challenges for IT professionals, educators, and content creators who want to stay within the law.

### Fair Use in Digital Contexts

Digital technology has made copying trivially easy and distribution instantaneous, which puts enormous pressure on fair use boundaries. Consider a few common scenarios:

* **Search engines** display thumbnail images and text snippets from websites. Courts have generally ruled this is fair use because it is transformative (helping users find information) and does not replace the original content.
* **Memes** often incorporate copyrighted images with new captions or contexts. Most memes probably qualify as fair use due to their transformative nature, though this has not been definitively tested in court.
* **Educational use** is often assumed to be automatically fair use, but that is a misconception. Photocopying an entire textbook chapter for a class, or uploading a full copyrighted article to a course website, may exceed fair use limits even in educational settings.

### Case Study 9.1 - The Google Books Scanning Project 📋

**The Situation:** Beginning in 2004, Google partnered with major research libraries to scan millions of books and make them searchable through Google Books. Users could search the full text of books and view short snippet results showing a few sentences around their search terms. For books still under copyright, Google displayed only these limited snippets, not the full text. Google did not obtain permission from the authors or publishers before scanning their works.

The Authors Guild filed a lawsuit in 2005, arguing that Google's mass scanning constituted copyright infringement on an unprecedented scale. The case wound through courts for over a decade. Google argued that its project was transformative: it created a searchable index of human knowledge, helped readers discover books they would then purchase, and provided accessibility benefits for visually impaired users through its text-to-speech features. The Authors Guild countered that Google was profiting commercially from unauthorized copies of copyrighted works and that the scanning project would reduce incentives for authors to create new works.

In 2015, the Second Circuit Court of Appeals ruled in Google's favor, finding that the project qualified as fair use. The court emphasized the transformative purpose of the search function, the limited amount of text displayed to users, and evidence that the project actually increased book sales rather than undermining them. The Supreme Court declined to hear the case, leaving the ruling in place.

**Stakeholders:**
* **Google** gained a massive searchable database and increased traffic to its platform, reinforcing its position as the world's information gateway
* **Authors and publishers** lost control over how their copyrighted works were used and received no direct compensation from the scanning
* **Researchers and the public** gained the ability to search millions of books instantly, a capability that previously did not exist
* **Libraries** preserved fragile collections digitally and expanded access to rare works
* **Visually impaired readers** gained access to books through text-to-speech features enabled by the digital scans

**Questions to Consider:**
1. The court found Google's use "transformative" because it created a new functionality (search) rather than substituting for the original books. Do you agree with this reasoning? Where would you draw the line between a transformative use and simple copying?
2. Consider this case from the perspective of a midlist author who earns modest royalties. Does the fact that the project may increase overall book sales adequately address the ethical concern of using their work without permission?
3. How might this ruling affect future cases involving large-scale data collection, including the AI training data disputes described later in this module?

### Open Source Licensing

Not everyone believes in restricting access to creative works. The **open source** movement represents a fundamentally different philosophy: that software (and increasingly other creative works) should be freely available for anyone to use, modify, and distribute. Open source is not the absence of licensing. It is a specific set of licensing models that define how freely shared works can be used.

The most common open source licenses fall into two categories:

* **Permissive licenses** (such as the MIT License and Apache License) allow nearly unrestricted use, including incorporating open source code into commercial products. The main requirement is attribution: you must credit the original creators.
* **Copyleft licenses** (such as the GNU General Public License, or GPL) require that any derivative work be released under the same license. This means that if you use GPL-licensed code in your software, your software must also be open source. This "viral" quality is intentional: it ensures that improvements to the codebase remain freely available.

The ethical arguments for open source are compelling. Proponents argue that software built collaboratively and shared freely accelerates innovation, reduces barriers to entry for new developers, and promotes transparency. When source code is public, anyone can audit it for security flaws or hidden behaviors.

However, open source raises its own ethical questions. Companies sometimes build profitable products on top of free open source code without contributing back to the community. Volunteer open source developers often burn out maintaining critical infrastructure that millions of people and businesses depend on. The **Creative Commons (CC)** licensing system extends similar principles to non-software works like textbooks (including this one), photographs, and music.

### Think About It 9.2 🧠

> Many of the tools you use every day, from web browsers to operating systems to programming languages, are built on open source code. Should companies that profit from open source software be ethically obligated to contribute back to the projects they depend on? Why or why not?

### Quick Check 9.2 ✅

1. List the four factors courts use to evaluate a fair use claim. Which factor do you think is most important in digital contexts, and why? *(Understand)*
2. A student uploads a full copyrighted documentary to a class discussion board so classmates can watch it for an assignment. Analyze whether this qualifies as fair use by applying the four-factor test. *(Analyze)*
3. What is the key difference between a permissive open source license (like MIT) and a copyleft license (like GPL)? Why does this distinction matter for a company building commercial software? *(Apply)*

---

## 9.3 Plagiarism, Piracy, and Competitive Intelligence

IP law sets the legal boundaries. But many of the most difficult decisions IT professionals face fall in gray areas where the law is ambiguous, varies by jurisdiction, or simply has not caught up with current practice. This section covers three areas where ethical reasoning matters as much as legal knowledge: plagiarism, digital piracy, and competitive intelligence practices like reverse engineering.

### Plagiarism in IT Contexts

**Plagiarism** is presenting someone else's work, ideas, or expressions as your own without proper attribution. In academic settings, plagiarism is a serious violation of integrity. In professional IT settings, it takes different forms: copying code from Stack Overflow without attribution, reusing a colleague's design work in a portfolio, or submitting vendor documentation as your own analysis.

Plagiarism and copyright infringement overlap but are not identical. You can plagiarize something that is not copyrighted (like an idea or a fact presented without attribution), and you can infringe copyright without plagiarizing (like copying a song you fully credit to the original artist but do not have permission to redistribute). The ethical issue with plagiarism is dishonesty: it misrepresents the origin of work and undermines trust.

For IT professionals, code plagiarism raises particular concerns. Open source code is meant to be reused, but even open source licenses typically require attribution. Copying proprietary code from a previous employer into a new project can violate trade secret protections and employment agreements. Understanding what you can reuse, and how to credit it properly, is a practical skill every IT worker needs.

### Digital Piracy

**Digital piracy** refers to the unauthorized copying, distribution, or use of copyrighted digital content, including software, music, movies, games, and e-books. The scale of digital piracy is enormous. Industry groups estimate billions of dollars in annual losses, though the exact figures are debated because not every pirated copy represents a lost sale.

The ethical arguments around piracy are more complex than they first appear. Those who oppose piracy argue that creators deserve to be compensated for their work, that piracy undermines the economic incentives for creating new content, and that it is simply a form of theft. Those who see piracy differently argue that digital copies are not like physical goods (copying a file does not deprive the owner of the original), that many people who pirate content could not or would not have paid for it anyway, and that restrictive pricing models and regional availability gaps push consumers toward piracy.

The **Digital Millennium Copyright Act (DMCA)**, passed in 1998, is the primary U.S. law addressing digital piracy. The DMCA criminalizes the circumvention of **digital rights management (DRM)** technologies and provides a "notice and takedown" process for copyright holders to request removal of infringing content from websites. Critics argue that the DMCA is overly broad, chilling legitimate uses like security research and archival preservation.

### Reverse Engineering and Competitive Intelligence

**Reverse engineering** is the process of analyzing a product to understand how it works, often to build a competing product or ensure compatibility. In IT, this might mean decompiling software, analyzing network protocols, or studying how a competitor's system handles data.

The legal status of reverse engineering depends heavily on context. In the United States, courts have generally allowed reverse engineering for purposes of achieving interoperability (making your software work with someone else's system) or conducting security research. However, the DMCA's anti-circumvention provisions create complications: if reverse engineering requires bypassing DRM or other technical protections, it may violate the law even if the underlying purpose is legitimate.

**Competitive intelligence** is the broader practice of gathering information about competitors to inform business strategy. Most competitive intelligence is perfectly legal and ethical: reading public filings, attending trade shows, analyzing publicly available products, and monitoring news coverage. The line gets crossed when companies use deceptive practices to obtain information, recruit employees primarily to extract trade secrets, or access proprietary systems without authorization.

### Trademark Infringement and Cybersquatting

While copyright and patent disputes get most of the headlines, trademark violations are common in the digital world. **Trademark infringement** occurs when someone uses a mark that is confusingly similar to an existing trademark in a way that is likely to mislead consumers. In IT contexts, this often involves domain names, app names, or website designs that imitate established brands.

**Cybersquatting** is the practice of registering domain names that incorporate well-known trademarks with the intent to profit from them, typically by selling the domain to the trademark holder at an inflated price. The **Anticybersquatting Consumer Protection Act (ACPA)** of 1999 and the **Uniform Domain-Name Dispute-Resolution Policy (UDRP)** administered by the Internet Corporation for Assigned Names and Numbers (ICANN) provide legal remedies for trademark holders whose names have been cybersquatted.

### Think About It 9.3 🧠

> A friend tells you they pirate all their software because they cannot afford to buy it. They argue that they are not hurting anyone since they would never have paid for it anyway. How would you respond? Does it matter whether the software is made by a large corporation or an independent developer?

### Quick Check 9.3 ✅

1. Explain the difference between plagiarism and copyright infringement. Can you commit one without the other? Give an example of each. *(Understand)*
2. A startup reverse-engineers a competitor's file format so that its own product can import the competitor's files. Analyze whether this practice is ethical by considering the interests of all stakeholders involved. *(Analyze)*
3. Apply the ethical frameworks from Module 1 (utilitarianism and deontology) to the debate over digital piracy. What does each framework say about the ethics of downloading copyrighted content without paying? *(Apply)*

---

## 9.4 AI and Intellectual Property: Uncharted Territory

The rise of generative AI has created some of the most challenging IP questions the legal system has ever faced. When an AI system produces a painting, writes a poem, or generates code, who owns the result? When AI companies train their models on billions of copyrighted works scraped from the internet, did they infringe copyright or engage in fair use? These questions are not hypothetical. They are being fought in courtrooms right now, and the answers will shape the future of creative work, software development, and the technology industry.

### Who Owns AI-Generated Works?

Under current U.S. copyright law, only works created by human beings can be copyrighted. The U.S. Copyright Office has consistently held that the connection between the human mind and creative expression is a fundamental requirement. In 2023, the Copyright Office issued guidance clarifying that purely AI-generated content cannot be registered for copyright protection. If you type a prompt into an image generator and it produces a picture, you do not own the copyright on that picture because you did not create the expressive elements yourself.

However, the situation becomes more complex when humans and AI collaborate. If a human author uses AI as a tool but makes substantial creative choices, such as selecting, arranging, and editing AI-generated elements into a larger work, those human-authored elements may be copyrightable. The Copyright Office has handled these cases on an individual basis, and the boundary between "human-authored with AI assistance" and "AI-generated" is not yet clearly defined.

This creates practical problems for IT professionals and businesses. If AI-generated code cannot be copyrighted, can competitors freely copy it? If a marketing team uses AI to create advertising images, does the company have any IP protection for those images? These uncertainties are already affecting business decisions.

### AI Training Data and Copyright

The other side of the AI-IP debate concerns the data used to train AI systems. Large language models and image generators are trained on enormous datasets that typically include copyrighted material: books, articles, photographs, artwork, and source code scraped from the internet. AI companies argue that this training process is fair use because the models learn patterns and concepts rather than storing or reproducing specific works. Critics argue that training on copyrighted material without permission is infringement, regardless of how the data is processed internally.

Several major lawsuits are testing these arguments. The *New York Times v. Microsoft and OpenAI* case, filed in late 2023, alleges that ChatGPT can reproduce substantial portions of *Times* articles verbatim, demonstrating that the model did more than simply "learn" from the content. Other cases brought by authors, visual artists, and music publishers raise similar claims against various AI companies. Getty Images sued Stability AI for training its image generator on millions of Getty's copyrighted photographs.

The outcome of these cases will have enormous consequences. If courts rule that AI training on copyrighted data is not fair use, AI companies may need to license training data, fundamentally changing the economics of AI development. If courts rule that training is fair use, creators may lose meaningful control over how their works are used in the age of AI.

### The Global Dimension

Different countries are taking different approaches. The European Union's AI Act includes provisions about transparency in training data, requiring companies to disclose what copyrighted material was used. Japan has taken a more permissive stance, generally allowing AI training on copyrighted works for the purpose of information analysis. These differences create challenges for global technology companies that must comply with varying legal frameworks across jurisdictions.

As you learned in Module 8, different regulatory philosophies reflect different ethical values. The EU's precautionary approach prioritizes creator rights and transparency. Japan's permissive approach prioritizes innovation and economic competitiveness. The United States is taking a case-by-case judicial approach, letting courts decide rather than passing comprehensive legislation. Each reflects a different set of assumptions about how to balance innovation against the rights of existing creators.

### Quick Check 9.4 ✅

1. Under current U.S. law, can a work generated entirely by AI receive copyright protection? Explain the reasoning behind this position. *(Understand)*
2. Compare the arguments made by AI companies (that training on copyrighted data is fair use) with the arguments made by copyright holders (that training without permission is infringement). Which of the four fair use factors supports each side? *(Analyze)*
3. A software developer uses an AI coding assistant to generate a function, then significantly modifies and integrates it into a larger program. Evaluate whether the developer should be able to claim copyright on the final product. What factors would you consider? *(Evaluate)*

---

## 9.5 Skills Lab 9A - Intellectual Property Analysis

**Goal:** Analyze a complex IP scenario involving multiple forms of intellectual property protection, fair use arguments, and AI-related ownership questions.

**Estimated time:** 90-120 minutes

### Scenario: TechCanvas and the AI Art Platform

TechCanvas is a mid-sized software company that has launched an AI-powered design platform called ArtForge. The platform allows users to type text prompts and receive AI-generated images, logos, and design layouts. ArtForge has become popular with small businesses, freelance designers, and marketing teams who use it to quickly produce visual content.

Several issues have emerged since ArtForge's launch. First, an independent investigation revealed that TechCanvas trained ArtForge's AI model on a dataset of 400 million images scraped from the internet, including copyrighted photographs from professional photographers, illustrations from working artists, and images from stock photography services. TechCanvas did not obtain permission from or compensate any of these creators. The company argues that scraping publicly available images for AI training is a transformative, fair use.

Second, a freelance graphic designer named Maria Delgado discovered that when she types her own name as part of a prompt, ArtForge generates images that closely resemble her distinctive illustration style. Maria has built her career and reputation on that style over fifteen years. She argues that ArtForge is effectively allowing anyone to produce knockoffs of her work. TechCanvas responds that artistic styles are not copyrightable and that ArtForge is simply a tool that learned general visual patterns.

Third, several small businesses that created logos and marketing materials using ArtForge are now discovering that they may not have clear copyright protection over the AI-generated designs. A competitor copied one company's ArtForge-generated logo almost exactly, and the company found it had limited legal recourse because the logo was generated by AI rather than created by a human designer.

### Part 1: Foundation (Aligns with LO1)

1. Identify each type of intellectual property relevant to this scenario (copyright, patent, trademark, trade secret). For each type, explain specifically how it applies to the situation described.
2. List all the stakeholders in this scenario. For each stakeholder, describe what they stand to gain or lose and which IP protections are most relevant to their interests.
3. The freelance designer Maria argues her illustration style is being copied. Under current IP law, is an artistic "style" protectable? Explain which type of IP protection (if any) might apply and why styles are treated differently from specific works.

### Part 2: Application (Aligns with LO2)

4. Apply the four-factor fair use test to TechCanvas's decision to train ArtForge on 400 million scraped images. Analyze each factor separately and then state your overall conclusion about whether the training qualifies as fair use.
5. The small businesses that used ArtForge to create logos are discovering they lack copyright protection. Analyze the ethical responsibilities TechCanvas has to its users. Should the company have disclosed the IP limitations of AI-generated content before users relied on it for business purposes?
6. Compare this scenario to the Google Books case discussed earlier in this module. What similarities and differences do you see? Does the Google Books ruling support or undermine TechCanvas's fair use argument?

### Part 3: Extension (Aligns with LO3)

7. Evaluate the competing interests in this scenario and propose a policy framework that balances the rights of original creators, AI companies, and end users of AI-generated content. Your proposal should address training data, generated output, and disclosure requirements.
8. Consider this scenario from an international perspective. If TechCanvas operates globally, how might the different approaches taken by the U.S., the EU, and Japan (as discussed in Section 9.4) affect the company's obligations? Evaluate whether a single global standard for AI and IP is desirable or whether regional differences serve an important purpose.

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

## 9.6 Summary and Retrieval 💡

### Key Concepts

* **Intellectual property law protects intangible creative and innovative works** through four main mechanisms: copyright (original expression), patents (inventions), trademarks (brand identity), and trade secrets (confidential business information). Each type covers different kinds of work and has different requirements and durations.

* **Fair use allows limited use of copyrighted material without permission**, but its boundaries are unpredictable. Courts weigh four factors: purpose and character of use, nature of the copyrighted work, amount used, and effect on the market. Digital technology has intensified fair use debates because copying and distribution have become effortless.

* **Open source licensing represents an alternative to traditional IP restrictions**, with permissive licenses (like MIT) allowing broad reuse and copyleft licenses (like GPL) requiring that derivative works remain open source. The open source philosophy prioritizes collaborative innovation and transparency.

* **Digital piracy, reverse engineering, and competitive intelligence** occupy gray areas where legal rules, ethical principles, and practical considerations do not always align. Understanding where the lines fall, and where they are genuinely uncertain, is essential for IT professionals.

* **AI has disrupted traditional IP frameworks.** Under current U.S. law, purely AI-generated works cannot be copyrighted. The legality of training AI models on copyrighted data is being tested in multiple high-profile lawsuits. Different countries are adopting different approaches, creating a complex global landscape for technology companies.

### Key Terms

**Section 9.1**
* **Intellectual property (IP):** Legal protections for intangible creative works, inventions, brand identities, and confidential business information.
* **Copyright:** Protection for original works of authorship fixed in tangible form, lasting the author's lifetime plus 70 years.
* **Work for hire:** A legal doctrine under which the employer, not the employee, owns the copyright for works created as part of employment.
* **Patent:** An exclusive right to make, use, and sell an invention for a limited period (typically 20 years).
* **Software patent:** A patent covering software-related innovations; controversial due to concerns about overly broad claims.
* **Trademark:** A word, phrase, symbol, or design that identifies the source of goods or services.
* **Trade secret:** Confidential business information that provides a competitive advantage, protected as long as it remains secret.
* **Defend Trade Secrets Act (DTSA):** A 2016 federal law providing a cause of action for trade secret misappropriation.

**Section 9.2**
* **Fair use:** A legal doctrine allowing limited use of copyrighted material without permission, evaluated by a four-factor test.
* **Open source:** A licensing philosophy that allows software to be freely used, modified, and distributed under specified conditions.
* **Permissive license:** An open source license (such as MIT or Apache) that allows broad reuse with minimal restrictions.
* **Copyleft license:** An open source license (such as GPL) that requires derivative works to be released under the same license.
* **Creative Commons (CC):** A licensing system extending open source principles to non-software creative works.

**Section 9.3**
* **Plagiarism:** Presenting someone else's work or ideas as your own without proper attribution.
* **Digital piracy:** Unauthorized copying, distribution, or use of copyrighted digital content.
* **Digital Millennium Copyright Act (DMCA):** A 1998 U.S. law that criminalizes circumvention of digital rights management and provides a notice-and-takedown process.
* **Digital rights management (DRM):** Technologies designed to control access to and use of copyrighted digital content.
* **Reverse engineering:** Analyzing a product to understand how it works, often for interoperability or competitive purposes.
* **Competitive intelligence:** The practice of gathering publicly available information about competitors to inform business strategy.
* **Cybersquatting:** Registering domain names incorporating well-known trademarks with intent to profit from them.
* **Anticybersquatting Consumer Protection Act (ACPA):** A 1999 law providing legal remedies against cybersquatting.
* **Uniform Domain-Name Dispute-Resolution Policy (UDRP):** An ICANN-administered process for resolving domain name disputes involving trademarks.

**Section 9.4**
* **AI-generated works:** Content produced by artificial intelligence systems, currently ineligible for U.S. copyright protection when created without substantial human creative input.
* **Training data:** The datasets used to train AI models, often including copyrighted material whose use is legally contested.

### Retrieval Practice

Try to answer these from memory before looking back at the module.

1. Name the four types of intellectual property and state what each one protects. Which type requires a formal application, and which is automatic?
2. What are the four factors courts consider when evaluating a fair use claim? Give a brief example of how one factor might weigh in favor of fair use and how the same factor might weigh against it.
3. Explain the current legal status of AI-generated works under U.S. copyright law. Why does this matter for businesses using AI tools to create content?

---

## 9.7 Discussion Prompt 💬

**Prompt:** AI companies argue that training their models on copyrighted material from the internet is fair use because the models learn general patterns rather than copying specific works. Copyright holders argue that using their work without permission to build commercial AI products is theft, regardless of how the technology processes the data internally.

Consider both sides of this debate. Where do you stand? Should AI companies be required to license the copyrighted material they use for training, or does the transformative nature of AI training justify treating it as fair use? Use at least one concept from this module (fair use factors, IP types, open source philosophy, or ethical frameworks from earlier modules) to support your reasoning. Address the strongest counterargument to your position.

**Guidelines:**
* Your initial post should be 200-300 words
* Reference at least one concept from this module and connect it to your reasoning
* Respond to at least two classmates with substantive engagement
* Consider how your position would affect different stakeholders: individual creators, AI companies, and the public

---

## Further Reading 📖

* **U.S. Copyright Office: "Copyright and Artificial Intelligence" (2023).** The Copyright Office's official guidance on the registration of works containing AI-generated material. Explains the current legal framework and the human authorship requirement. Available free at copyright.gov.

* **Creative Commons: "About the Licenses."** A clear, accessible explanation of how Creative Commons licenses work and how to choose one for your own work. Essential reading for anyone creating or using open educational resources. Available free at creativecommons.org.

* **Electronic Frontier Foundation: "Fair Use FAQ."** A practical guide to understanding fair use from one of the leading digital rights organizations. Includes real-world examples and common misconceptions. Available free at eff.org.

* **Open Source Initiative: "The Open Source Definition."** The foundational document defining what qualifies as open source software, including the ten criteria a license must meet. Useful for understanding the philosophical and legal foundations of the open source movement. Available free at opensource.org.

* **Lemley, M.A. and Casey, B. (2020). "Fair Learning."** A law review article examining how fair use doctrine should apply to machine learning training. Provides a thorough legal analysis of the arguments on both sides. Available through academic databases.

---

## Looking Ahead ⏩

In Module 10, you will shift from questions of ownership to questions of expression. Who gets to say what online, and what happens when speech causes harm? Module 10 examines the boundaries of the First Amendment in digital spaces, the classification of hate speech and defamation, the ethics of internet anonymity, and the growing tension between employee monitoring and workplace privacy. You will also explore how AI-generated deepfakes and automated content moderation systems are complicating these debates in ways the law was never designed to handle.
