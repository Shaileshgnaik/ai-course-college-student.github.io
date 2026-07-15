# Module 08 — Responsible AI

## Learning Objectives

By the end of this module students will:

- Understand the ethical principles behind responsible AI development and use
- Identify types of AI bias and their real-world impact
- Evaluate AI systems for fairness, transparency, and accountability
- Apply responsible AI principles in their own AI use

---

## Topics Covered

### 1. What is Responsible AI?

Responsible AI is a framework for ensuring that AI systems are developed and deployed in ways that are fair, transparent, accountable, safe, and privacy-preserving. It acknowledges that AI systems are not neutral tools — they encode the values, assumptions, and limitations of their creators and training data, and they can cause real harm when those limitations are not addressed.

Microsoft, Google, and the EU have all published responsible AI frameworks. Despite different terminology, they converge on similar principles: fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability.

### 2. Fairness and Bias in AI Systems

AI bias occurs when a model systematically produces outputs that unfairly advantage or disadvantage particular groups. Bias typically enters through training data, but can also be introduced through problem framing, feature selection, and evaluation choices.

**Types of bias:**

**Historical bias:** The training data reflects historical human inequities. A hiring model trained on historical hiring decisions will learn those decisions — including discriminatory ones.

**Representation bias:** Some groups are underrepresented in training data. Early facial recognition systems had significantly higher error rates for darker-skinned faces because training datasets were predominantly lighter-skinned.

**Measurement bias:** Proxies for the outcome of interest are systematically skewed. Using zip code as a proxy for creditworthiness can perpetuate racial segregation.

**Feedback loop bias:** AI predictions influence human behaviour, which generates new training data, reinforcing the original prediction. Predictive policing systems that direct police to high-crime areas generate more arrests in those areas, confirming the prediction.

**Real-world examples:** Amazon's scrapped AI recruiting tool (downgraded women's CVs), COMPAS recidivism prediction (higher false positive rates for Black defendants), and facial recognition used in law enforcement (multiple wrongful arrests of Black men).

### 3. Transparency and Explainability

Transparency means being open about how an AI system works — what data it was trained on, how it makes decisions, and what its limitations are. Explainability means being able to explain a specific decision in terms a human can understand.

These properties matter because people affected by AI decisions deserve to understand why a decision was made and have a meaningful way to challenge it. The EU AI Act (2024) legally requires explainability for high-risk AI systems (credit scoring, hiring, medical diagnosis).

"Black box" AI — systems where even the developers cannot explain specific outputs — is increasingly problematic in regulated domains.

### 4. Privacy and Data Protection

AI systems are trained on data, and that data often contains personal information. Key privacy risks:

**Data leakage:** Models can sometimes reproduce training data when prompted. Researchers have extracted personal information from GPT models by carefully crafting prompts.

**Re-identification:** Anonymised datasets can sometimes be de-anonymised when combined with other data sources.

**Consent:** Users whose data was scraped to train models often had no meaningful opportunity to consent.

**Surveillance:** AI-powered surveillance systems (facial recognition, behaviour tracking) can operate at scales that would have been impossible without AI.

Key regulations: GDPR (Europe), DPDP Act (India), CCPA (California). These set rights over personal data and obligations for AI systems that process it.

### 5. AI Safety and Alignment

AI safety is concerned with ensuring AI systems do what their designers intend and do not cause harm. Alignment refers to the challenge of ensuring an AI's goals are aligned with human values.

Current AI systems can exhibit problematic behaviours without any malicious intent: generating harmful content, being manipulated by adversarial inputs, pursuing proxies for goals that lead to unintended outcomes. These are primarily engineering challenges today, but they become existentially important as AI systems become more capable and autonomous.

### 6. Academic Integrity and AI

Using AI in academic work raises specific integrity questions:

- **Disclosure:** Most institutions are moving toward requiring disclosure of AI use, not prohibiting it
- **Authorship:** Work presented as your own must reflect your understanding; AI-generated content submitted verbatim without disclosure is academic misconduct
- **Verification:** You are responsible for the accuracy of everything you submit, whether AI-assisted or not
- **Skill development:** Over-reliance on AI in learning contexts can prevent you from developing core skills you'll need later

The key question is not "did I use AI?" but "did I understand, evaluate, and take responsibility for everything I submitted?"

### 7. AI Governance and Regulation (EU AI Act, etc.)

Governments worldwide are developing AI governance frameworks:

**EU AI Act (2024):** The first comprehensive AI law. Classifies AI systems by risk level — prohibited applications (social scoring, real-time biometric surveillance), high-risk applications (hiring, credit, education — require transparency and human oversight), limited risk (chatbots must disclose they're AI), minimal risk (spam filters, video games — no requirements).

**India:** Developing an AI governance framework under the Digital India initiative. The Indian government has emphasised responsible AI development aligned with Indian values and development goals.

**USA:** Executive orders and agency-level guidelines, but no comprehensive AI law yet as of 2025.

**International:** UNESCO adopted a global Recommendation on the Ethics of AI in 2021, signed by 193 member states.

### 8. Building Ethical AI Habits

Responsible AI is not just for AI developers — it applies to every person who uses AI tools.

**As an AI user:**
- Verify AI outputs before acting on them or sharing them
- Disclose AI use appropriately
- Do not use AI to generate harmful, misleading, or abusive content
- Be aware of who owns the data you put into AI tools
- Consider the impact of AI-generated content on others

**As a future professional:**
- Question AI systems that affect people — ask about training data, accuracy rates, and bias testing
- Advocate for transparency in AI systems used in your organisation
- Understand the legal and ethical obligations in your domain

---

## Demonstrations

- Demonstrating and discussing AI bias in generated text and images
- Exploring Microsoft's Responsible AI principles and tools
- Analysing the COMPAS recidivism case study

## Hands-on Activities

- Analyse an AI system for potential bias — document your findings
- Write a 1-page AI usage policy for a fictional company
- Class debate: "Should AI be used in university admissions?"

## Assignment

Choose a real-world AI controversy. Write a 500-word analysis covering what happened, the ethical issues, who was harmed, and what should change. See `../../assessments/assignments/README.md` for full brief.

## Additional Resources

- [Microsoft Responsible AI](https://www.microsoft.com/en-us/ai/responsible-ai)
- [EU AI Act Summary](https://digital-strategy.ec.europa.eu/en/policies/european-approach-artificial-intelligence)
- [The Alignment Problem — Brian Christian](https://brianchristian.org/the-alignment-problem/)

---

*Previous: [Module 07 — AI for Programming](../07-AI-for-Programming/README.md)  |  Next: [Module 09 — Future of AI](../09-Future-of-AI/README.md)*
