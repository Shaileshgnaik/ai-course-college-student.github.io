---
layout: default
title: "Student Study Assistant"
parent: Projects
nav_order: 2
permalink: /projects/student-study-assistant/
---

# Project: Student Study Assistant

**Difficulty:** Beginner to Intermediate
**Estimated time:** 4–6 hours
**Tools:** ChatGPT, Microsoft Copilot, or any LLM

---

## Problem Statement

Students spend enormous time trying to understand complex topics, summarise readings, and prepare for exams — but often don't know how to study effectively.

This project uses AI to create a personalised study assistant tailored to a specific subject you're currently studying.

---

## What You'll Build

A complete AI-powered study toolkit for one of your current subjects, including:
1. A subject-specific prompt library (15 prompts)
2. An AI-generated study guide for one topic
3. A practice exam with 20 questions and answer key
4. A concept explanation library (10 key terms explained 3 ways)
5. A weekly study plan

---

## Step-by-Step Guide

### Step 1 — Choose Your Subject (15 min)
Pick one subject you are currently studying. Identify:
- The subject name and your current topic/chapter
- 10 key concepts or terms you need to understand
- Any upcoming exam or assignment

### Step 2 — Build Your Prompt Library (60 min)
Create 15 prompts for your subject. Use this template for each:

| # | Use Case | Your Optimised Prompt |
|---|----------|----------------------|
| 1 | Explain a concept simply | |
| 2 | Give a real-world example | |
| 3 | Compare two related concepts | |
| 4 | Generate practice questions | |
| 5 | Summarise a chapter | |
| 6 | Create a mind map outline | |
| 7 | Explain why this matters | |
| 8 | Identify common mistakes | |
| 9 | Create a mnemonic | |
| 10 | Predict exam questions | |
| 11 | Explain in simple language | |
| 12 | Create a timeline/sequence | |
| 13 | Solve a practice problem | |
| 14 | Give a counterargument | |
| 15 | Connect to another topic | |

Test each prompt and refine until the output is genuinely useful.

### Step 3 — Generate a Study Guide (45 min)
Choose your most challenging topic and generate a complete study guide:
```
You are a tutor helping a [your year] year [your course] student prepare for an exam on [topic].
Create a complete study guide that includes:
1. Overview (3 sentences)
2. Key concepts (each explained in 2-3 sentences)
3. Important formulas/frameworks/dates (as applicable)
4. Common exam questions on this topic
5. Common mistakes students make
6. A 5-point summary to review the night before the exam
```

Review the guide. Annotate it with corrections, additions, or clarifications.

### Step 4 — Practice Exam Generator (30 min)
```
Create a 20-question practice exam on [topic] for a [your year] year [your course] student.
Include:
- 8 multiple choice questions
- 6 short answer questions (2-3 sentences expected)
- 4 application questions (apply the concept to a scenario)
- 2 analysis questions (compare, evaluate, or critique)
Provide an answer key separately.
```

Take the exam yourself before looking at the answer key.

### Step 5 — Concept Explanation Library (45 min)
For each of your 10 key terms, use this prompt:
```
Explain [concept] three ways:
1. In one sentence for a complete beginner
2. In a paragraph with a real-world example
3. Technically, as it would appear in an exam answer
```

### Step 6 — Weekly Study Plan (20 min)
```
Create a 2-week study plan for [subject] with [X hours] available per day.
My exam is on [date]. Topics to cover: [list your topics].
Include: daily tasks, practice questions, review sessions, and rest days.
```

---

## Deliverables

- [ ] Prompt library (15 prompts, tested and documented)
- [ ] Study guide (AI-generated + your annotations)
- [ ] Practice exam (20 questions) + answer key + your score
- [ ] Concept explanation library (10 terms × 3 explanations)
- [ ] Weekly study plan
- [ ] Reflection: Did AI help you understand the subject better? What would you improve?

---

## Extension Tasks

- Use Copilot to create a PowerPoint presentation summarising the topic for a 5-minute class presentation
- Ask AI to generate flashcards: *"Create 20 flashcard pairs (question/answer) for [topic]"*
- Ask AI to quiz you interactively: *"Quiz me on [topic]. Ask one question at a time and wait for my answer before revealing if I'm correct."*
