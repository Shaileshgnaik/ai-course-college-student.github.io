# Lab 02 — Prompt Engineering

**Duration:** 75 minutes
**Module:** Follows Module 05 — Prompt Engineering
**Tools needed:** ChatGPT or Microsoft Copilot

---

## Objectives

By the end of this lab you will:
- Apply zero-shot, few-shot, and chain-of-thought prompting techniques
- Iteratively refine prompts to improve AI output quality
- Build a personal prompt library for your area of study

---

## Part 1: Weak vs Strong Prompts (20 minutes)

For each weak prompt below, rewrite it as a strong prompt and compare the AI's responses.

**Instructions:**
1. Send the weak prompt to the AI and note the response quality (1-5 scale)
2. Rewrite the prompt using what you know about effective prompting
3. Send the improved prompt and rate the response again

| # | Weak Prompt | Your Improved Prompt | Weak Score | Strong Score |
|---|-------------|---------------------|-----------|-------------|
| 1 | "Write about climate change" | | | |
| 2 | "Help me study" | | | |
| 3 | "Make my resume better" | | | |
| 4 | "Explain quantum computing" | | | |
| 5 | "Give me interview tips" | | | |

**Strong prompt formula to use:**
```
[Role] + [Task] + [Context] + [Format] + [Constraints]
```

Example: *"You are a career coach. Write 5 interview tips for a final-year computer science student applying for their first software development internship. Format as a numbered list. Keep each tip under 30 words."*

---

## Part 2: Prompting Techniques (30 minutes)

### 2A — Zero-Shot Prompting
Ask the AI to do something with no examples:

*"Classify the following sentence as Positive, Negative, or Neutral: 'The new AI features in the app are interesting but sometimes unreliable.'"*

Note the response. Did it classify correctly?

---

### 2B — Few-Shot Prompting
Now give the AI examples before asking:

```
Classify each sentence as Positive, Negative, or Neutral.

Sentence: "I love how fast this AI responds." → Positive
Sentence: "The output was completely wrong." → Negative
Sentence: "The AI generated a response." → Neutral

Now classify: "The new AI features in the app are interesting but sometimes unreliable."
```

Compare the result to 2A. Was few-shot more accurate?

---

### 2C — Chain-of-Thought Prompting
Use step-by-step reasoning for a logic problem:

```
A student has 5 assignments due this week. Each takes 2 hours. 
They have 3 hours free on Monday, 4 hours on Wednesday, and 2 hours on Friday.
Think step by step: can they complete all assignments before the Friday deadline?
```

Notice how the AI reasons through the problem rather than guessing.

---

### 2D — Role Prompting
Ask the AI to adopt a persona:

First, ask normally: *"What should I know before a job interview?"*

Then use role prompting: *"You are a senior recruiter at a top tech company who has interviewed hundreds of candidates. What are the top 5 mistakes candidates make, and how should they be avoided? Speak directly to the candidate."*

Compare the tone, depth, and usefulness of both responses.

---

## Part 3: Build Your Prompt Library (25 minutes)

Create a personal prompt library of 8 prompts useful for YOUR area of study.

**Prompt Library Template:**

| # | Use Case | Your Optimised Prompt | Notes |
|---|----------|----------------------|-------|
| 1 | Summarise a research paper | | |
| 2 | Explain a difficult concept | | |
| 3 | Generate practice exam questions | | |
| 4 | Review my written work | | |
| 5 | Help plan a project | | |
| 6 | Draft a professional email | | |
| 7 | Prepare for a presentation | | |
| 8 | [Your own use case] | | |

Test each prompt and refine based on the output you receive.

---

## Lab Submission

Submit:
1. Your completed Weak vs Strong Prompts table (Part 1)
2. Your observations from each technique in Part 2 (2–3 sentences per technique)
3. Your completed Prompt Library (Part 3)

**Grading criteria:**
- Prompt improvement demonstrated with before/after (4 marks)
- All 4 techniques tested with observations (4 marks)
- Prompt library completed and tested (2 marks)
