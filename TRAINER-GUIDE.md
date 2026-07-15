# Trainer Guide

## Before the Course

- Review all module READMEs and prepare your demo accounts
- Set up and test: ChatGPT, Microsoft Copilot, GitHub Copilot, Google Colab
- Share [SETUP.md](SETUP.md) with students **at least 3 days before Week 1** so they arrive ready
- Clone the repo and familiarise yourself with the lab guides in `labs/`
- Ensure students have access to required tools (see SETUP.md)
- Print or share the [GLOSSARY.md](GLOSSARY.md) as a take-home reference

## Delivery Format

- Each module is designed for a **2–3 hour session**
- Recommended flow: **Slides (30 min) → Live Demo (30 min) → Hands-on Exercise (45 min) → Debrief (15 min)**
- Encourage students to try prompts in real-time during demos — don't just watch
- Pair students for exercises wherever possible — peer learning accelerates understanding
- Keep a running "parking lot" on the whiteboard for questions to address at the end

## Class Size

- Optimal: 20–40 students
- For groups > 40: add a co-trainer or TA for lab sessions
- For groups < 15: increase discussion time; students can present their exercise outputs

---

## Module-by-Module Trainer Notes

### Module 01 — Introduction to AI

**Key message:** AI is already everywhere in students' lives — this module makes the invisible visible.

**Tips:**
- Open with a live poll: "Which of these apps uses AI?" (Spotify, Netflix, Google Maps, Instagram) — nearly all of them do
- Avoid going deep on technical concepts; this is an orientation session
- The "AI Scavenger Hunt" exercise works well as an icebreaker

**Common questions:**
- *"Is AI going to take my job?"* — Redirect to Module 09 and 10; for now, focus on AI as a tool
- *"Is ChatGPT the same as AI?"* — Use this to explain the difference between a tool and the underlying technology

**Demo tip:** Open ChatGPT, Copilot, and Gemini side by side and ask the same question to all three — students find the comparison instantly engaging.

---

### Module 02 — Machine Learning Fundamentals

**Key message:** Machines learn from examples, just like humans — but at massive scale.

**Tips:**
- Use Google Teachable Machine for the hands-on exercise — it requires no coding and produces visible, satisfying results in minutes
- Avoid heavy math; focus on intuition (e.g., "training" = showing the computer thousands of examples)
- The Kaggle dataset exploration exercise works well in pairs

**Common questions:**
- *"Do I need to know maths for ML?"* — Not for this course; understanding the concepts is the goal
- *"What language do ML engineers use?"* — Mostly Python; introduce this in Module 07

**Demo tip:** Train a Teachable Machine image classifier live in the session using your webcam — classify hand gestures (thumbs up/down). Students can replicate it immediately on their laptops.

---

### Module 03 — Deep Learning & Neural Networks

**Key message:** Deep learning is what makes modern AI so powerful — and Transformers are the engine behind everything students use.

**Tips:**
- TensorFlow Playground (playground.tensorflow.org) is excellent for visualising how training works — run it live while explaining
- Keep the math conceptual: "more layers = can learn more complex patterns"
- The Transformer section is the most important — connect it explicitly to GPT and Copilot (which students already know)

**Common questions:**
- *"How many layers does GPT-4 have?"* — Exact architecture is not public, but frame it: hundreds of layers, billions of parameters
- *"Can I train a neural network myself?"* — Yes, in Google Colab with 10 lines of code; point to Module 07

**Demo tip:** Show the TensorFlow Playground with a spiral dataset — start with no hidden layers (fails), add 2 layers (succeeds). The visual "aha" moment is very effective.

---

### Module 04 — Generative AI & LLMs

**Key message:** LLMs don't "know" things — they predict the most likely next word, at massive scale. Understanding this explains both their power and their limits.

**Tips:**
- Live demo is essential — show ChatGPT, Copilot, and image generation (DALL-E or Copilot Designer) side by side
- Demonstrate a hallucination deliberately: ask an LLM about a fake person or event and show it confidently inventing details
- Discuss token limits practically: paste a long article and show what happens when the context is exceeded

**Common questions:**
- *"Is the AI conscious? Does it understand?"* — No; it predicts patterns. It doesn't "understand" in the human sense
- *"Which LLM is best?"* — They differ by use case; that's a good segue into Module 05

**Demo tip:** Ask the same creative prompt to 3 different models (ChatGPT, Copilot, Gemini) in the same session. The differences in style and quality spark great discussion.

---

### Module 05 — Prompt Engineering

**Key message:** The quality of your prompt determines the quality of your output — prompt engineering is a learnable, high-value skill.

**Tips:**
- Do live iterative prompting: start with a vague prompt, show the weak result, then refine it step by step — very impactful
- The "5 Weak Prompts" rewrite exercise is the best exercise in the course — give students 10 minutes and then share results
- Emphasise that prompt engineering is not about tricks — it's about being precise and giving the AI the context it needs

**Common questions:**
- *"Will prompt engineering still matter when AI gets smarter?"* — Yes, but the skills will evolve; clear communication always matters
- *"Is there a 'correct' prompt?"* — No; there's a spectrum from weak to strong, and iteration is the key skill

**Demo tip:** Use the "before/after" prompt structure live on screen:  
Before: *"Write something about climate change"*  
After: *"You are an environmental science professor. Write a 200-word explainer on climate change for first-year students, using no jargon. End with one practical action students can take."*  
The contrast is striking and immediately memorable.

---

### Module 06 — Microsoft Copilot

**Key message:** Copilot is a productivity multiplier — it doesn't replace thinking, it removes the friction around writing, formatting, and analysis.

**Tips:**
- Students need a Microsoft 365 account with Copilot enabled. Check this before the session. If unavailable, use copilot.microsoft.com as a fallback for all exercises
- Walk through Word, Excel, and PowerPoint step by step — don't assume familiarity
- The internship application package assignment (cover letter + skills summary + intro deck) is highly motivating for students

**Common questions:**
- *"Is this different from ChatGPT?"* — Copilot is integrated into the Microsoft 365 apps and has access to your documents; ChatGPT doesn't
- *"Can Copilot access my personal files?"* — Only with explicit permission via Microsoft 365; explain the privacy model

**Demo tip:** Generate a Word document from 5 bullet points live — students are consistently impressed by the speed. Then show tracked changes and how to accept/reject suggestions.

---

### Module 07 — AI for Programming

**Key message:** GitHub Copilot is like pair programming with an expert who never gets tired — but you are still the engineer; you must review everything it produces.

**Tips:**
- Use VS Code with GitHub Copilot live — write a Python function from a comment and let Copilot complete it
- Deliberately include a bug in Copilot's output and ask students to find it — reinforces critical review
- The "take a broken Python script and fix it with AI" exercise is excellent for building debugging intuition

**Common questions:**
- *"Will AI replace programmers?"* — Frame it as a tool that makes programmers more productive; junior roles may change but engineering judgment is irreplaceable
- *"Can I use Copilot in exams?"* — Depends on institution policy; responsible use means understanding what the code does

**Setup note:** Students need the GitHub Student Developer Pack approved before this session. Remind them at the end of Module 06 to apply if they haven't already.

**Demo tip:** Start a Python script from scratch using only comments as prompts — write `# function to read a CSV file and return average of a column` and let Copilot generate it. Then run the code to show it actually works.

---

### Module 08 — Responsible AI

**Key message:** AI amplifies human choices — both good and bad. Responsible use is a skill, not just a rule.

**Tips:**
- Use case studies to drive discussion rather than lecturing — students engage far more with real examples
- The "AI controversy analysis" assignment works best when students choose their own topic
- The debate format ("Should AI be used in university admissions?") generates excellent participation — split the room into for/against

**Common questions:**
- *"Who is responsible when AI makes a mistake?"* — This is intentionally an open question; use it to introduce AI governance
- *"Should I tell my professor I used AI?"* — Yes — transparency and disclosure are part of responsible use

**Sensitive topics:** Facial recognition bias, AI in criminal justice, and deepfakes can prompt strong reactions. Welcome the emotion — this module is meant to engage values, not just facts.

---

### Module 09 — Future of AI

**Key message:** AI is moving fast — careers, industries, and society will look very different in 10 years. The goal is to develop informed perspectives, not predictions.

**Tips:**
- Use this module to connect back to students' own disciplines — ask each student to think about their own field
- AI agents demos are compelling: show an AI completing a multi-step task autonomously (booking, research, writing)
- Keep the discussion grounded — acknowledge uncertainty rather than making confident predictions

**Common questions:**
- *"When will AGI arrive?"* — Genuinely uncertain; frame the range of expert opinions without advocating for one
- *"Should I be worried about AI?"* — Acknowledge legitimate concerns while focusing on agency: students who understand AI are better positioned than those who don't

**Demo tip:** Show a live AI agent completing a multi-step task (e.g., researching a topic, summarising findings, drafting an email). The gap between this and "chatbot" is what makes the future feel real.

---

### Module 10 — AI Careers & Roadmap

**Key message:** AI skills are now a baseline expectation across almost every career — the question is how deep to go, not whether to start.

**Tips:**
- Make this session personal — ask each student to identify their target career and then discuss how AI intersects with it
- The "AI Career Starter Pack" assignment (resume + LinkedIn + 3-month plan) is the most career-relevant assignment in the course; give it enough time
- Share your own career story — how you got into AI training and what you wish you'd known

**Common questions:**
- *"Do I need a computer science degree for an AI career?"* — Not necessarily; many AI roles are domain-specific (AI in healthcare, law, marketing, etc.)
- *"Where do I start after this course?"* — Point to the certifications table in the module README and encourage one concrete next step

**Closing ritual:** Ask each student to write down one AI tool they'll use this week and share it with the group. Ends the course on a practical, forward-looking note.

---

## Final Project Guidance

- Announce the project brief at the end of **Module 05** (Week 5)
- Students choose from the `projects/` folder or propose their own (trainer approval required)
- Final presentations in **Module 10** — 5 minutes per student or group
- Use the rubric in `assessments/project-rubrics/` for consistent grading

## Assessment Overview

| Component | Weight | Timing |
|-----------|--------|--------|
| Weekly quizzes (10 × 1%) | 10% | End of each module |
| Lab exercises (6 labs) | 20% | During lab sessions |
| Module assignments (10 × 3%) | 30% | Due before next module |
| Final project | 40% | Presented in Module 10 |

## Tools Required (Trainer Setup)

| Tool | Purpose | Free Tier? |
|------|---------|------------|
| ChatGPT | Generative AI demos | Yes |
| Microsoft Copilot | Office AI integration | Yes (limited) |
| GitHub Copilot | AI coding assistant | Yes (students via GitHub Education) |
| Google Colab | Python ML notebooks | Yes |
| Hugging Face | Model exploration | Yes |
| TensorFlow Playground | Neural network visualisation | Yes (browser-based) |
| Google Teachable Machine | No-code ML demo | Yes (browser-based) |
