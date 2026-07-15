---
layout: default
title: "Sample Answers — Modules 06, 07, 09, 10"
permalink: /assessments/sample-answers/module-06/
---

# Sample Answers — Modules 06, 07, 09 & 10

These modules involve practical deliverables (documents, code, presentations, career packs) rather than written essays, so the sample answers focus on **what excellent work looks like** with annotated rubric guidance and key diagrams.

---

## Module 06 — Internship Application Package

**What excellent work looks like:**

```mermaid
graph LR
    subgraph Word["📄 Cover Letter (Word)"]
        W1["Specific role named"]
        W2["Relevant skills matched to JD"]
        W3["Professional but personal tone"]
        W4["Under 200 words"]
    end
    subgraph Excel["📊 Skills Summary (Excel)"]
        E1["Skill name"]
        E2["Level: Beginner/Int/Adv"]
        E3["Evidence: project or cert"]
        E4["AI tools column included"]
    end
    subgraph PPT["🎨 Intro Deck (PowerPoint)"]
        P1["Slide 1: Name + tagline"]
        P2["Slide 2: Top 3 skills with examples"]
        P3["Slide 3: What I'm looking for"]
    end

    style Word fill:#ddf4ff,stroke:#0969da
    style Excel fill:#dafbe1,stroke:#2da44e
    style PPT fill:#fff8c5,stroke:#d4a72c
```

**Key differentiators for an A grade:**
- Cover letter references a specific company and role — not a template
- Skills table includes AI tools (Copilot, ChatGPT, GitHub Copilot) with evidence
- Intro deck has a clear personal brand, not just a list of facts
- Student documents which parts were AI-generated and which were personalised

<div class="tip-box">
<strong>💡 Examiner Tip:</strong> The most common weakness is submitting verbatim Copilot output without personalisation. If the cover letter could belong to any student, it scores in the C range. Personalisation is what separates a B from an A.
</div>

---

## Module 07 — AI-Assisted Mini Project

**What excellent work looks like — Python Quiz App example:**

```mermaid
flowchart TD
    A["📝 Comment-driven prompt\n# Quiz app that loads questions from CSV\n# Tracks score and shows final result"] --> B["🤖 GitHub Copilot generates\nfirst version of the code"]
    B --> C{"Does it run\ncorrectly?"}
    C -->|"Yes"| D["Review for edge cases\nWhat if CSV is empty?\nWhat if answer is wrong type?"]
    C -->|"No"| E["Debug with Copilot Chat\n'Fix this error: ...'"]
    E --> C
    D --> F["Add docstrings\n'Document each function'\nvia Copilot"]
    F --> G["Write README\n'Explain what this does\nand how to run it'"]
    G --> H["📦 Final submission\n.py file + README + reflection"]

    style A fill:#f6f8fa,stroke:#d0d7de
    style B fill:#ddf4ff,stroke:#0969da
    style H fill:#dafbe1,stroke:#2da44e
```

**Reflection — what to document:**
- What % of code did Copilot generate? (be honest — 70%+ is fine)
- What did you have to fix? (typos, logic errors, missing edge cases)
- What did you learn from reviewing the AI's code?
- Would you have built this without AI assistance? How long would it have taken?

<div class="tip-box">
<strong>💡 Examiner Tip:</strong> A student who submits Copilot-generated code with a thoughtful reflection that identifies 3 specific errors they caught scores higher than a student who writes everything manually but submits no reflection. The assignment measures AI literacy, not just coding ability.
</div>

---

## Module 09 — Future of AI Industry Brief

**Structure of an excellent 1-page brief:**

```mermaid
graph TD
    A["📄 Future of AI in Healthcare\n1-page brief"] --> B["Industry Context\n2 sentences — what AI already does in this field"]
    A --> C["Two Current Changes\nSpecific roles/tasks being transformed\nwith named AI tools or examples"]
    A --> D["One Automation Prediction\nA specific task likely automated\nin 5-10 years — with reasoning"]
    A --> E["One New Role/Skill\nWhat will emerge because of AI\nthat doesn't exist yet"]
    A --> F["Personal Recommendation\nWhat should students do NOW\n— specific and actionable"]

    style A fill:#0969da,color:#fff,stroke:#0550ae
    style F fill:#dafbe1,stroke:#2da44e
```

**Example of a strong personal recommendation (Healthcare):**
> "Students entering healthcare should enrol in at least one AI in Medicine course (e.g., Stanford's AI in Healthcare on Coursera) before graduation. Learning to interpret AI-generated diagnostic suggestions — not just trust them — will be a baseline clinical competency within a decade."

**Example of a weak recommendation (scores 0/2):**
> "Students should learn about AI and prepare for changes in their field."

<div class="tip-box">
<strong>💡 Examiner Tip:</strong> The recommendation is the most valuable section to the student's future employer — it shows independent thinking. Vague advice scores 0. Specific, evidenced recommendations (name the course, the certification, the skill) score 2/2.
</div>

---

## Module 10 — AI Career Starter Pack

**What excellent work looks like:**

```mermaid
graph LR
    subgraph Resume["📄 Resume"]
        R1["AI Skills section\n(tools + techniques)"]
        R2["Projects section\ncourse projects listed"]
        R3["Certifications\nat least 1 AI cert"]
    end
    subgraph LinkedIn["💼 LinkedIn About"]
        L1["Opening hook\n(not 'I am a student')"]
        L2["What you're learning\nand passionate about"]
        L3["AI tools you use\nin your studies/work"]
        L4["What you're looking for"]
    end
    subgraph Roadmap["🗺️ 3-Month Roadmap"]
        M1["Month 1: Certification goal\nAI-900 or Google AI Essentials"]
        M2["Month 2: Build one project\nfrom the projects/ folder"]
        M3["Month 3: Apply for roles\nor internships"]
    end

    style Resume fill:#ddf4ff,stroke:#0969da
    style LinkedIn fill:#dafbe1,stroke:#2da44e
    style Roadmap fill:#fff8c5,stroke:#d4a72c
```

**Strong AI Skills section example for resume:**

```
AI & Productivity Tools
• Generative AI: ChatGPT (GPT-4o), Microsoft Copilot, Claude
• Prompt Engineering: zero-shot, few-shot, chain-of-thought
• AI Coding: GitHub Copilot (Python, JavaScript)
• Microsoft 365 Copilot: Word, Excel, PowerPoint, Teams
• ML Tools: Google Colab, Kaggle, Teachable Machine
• Certifications: Microsoft AI-900 (in progress)
```

<div class="tip-box">
<strong>💡 Examiner Tip:</strong> "Familiar with AI tools" is the weakest possible AI skills entry — every student can write that. Name the specific tools, name the techniques, and where possible name a project where you used them. Recruiters scan résumés in 6 seconds — specificity is what stops the scroll.
</div>
