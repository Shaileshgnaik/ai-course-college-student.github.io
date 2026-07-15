---
layout: default
title: "Campus Chatbot"
permalink: /projects/campus-chatbot/
---

# Project: Campus Chatbot

**Difficulty:** Intermediate
**Estimated time:** 5–7 hours
**Tools:** ChatGPT or Microsoft Copilot (for prompt design), optionally Python

---

## Problem Statement

New students often struggle to find basic information about their college — timetables, departments, facilities, events, and processes. A well-designed AI chatbot could answer 80% of common student queries instantly.

This project designs and tests a campus information chatbot using prompt engineering — no coding required for the core deliverable, but a Python extension is available.

---

## What You'll Build

A fully designed, tested campus chatbot including:
1. A system prompt that configures the AI as a campus assistant
2. A knowledge base of 20 Q&A pairs for your college
3. A test suite of 15 conversation scenarios
4. An evaluation report on the chatbot's accuracy and limitations
5. (Optional) A basic Python interface

---

## Step-by-Step Guide

### Step 1 — Define Your Chatbot (20 min)
Decide on the scope of your chatbot:

```
Chatbot Name: [e.g., "CollegeBot", your college's name + "Assistant"]
College: [Your college name]
Primary audience: [First-year students / all students / prospective students]
Topics to cover: [List 5-8 topic areas, e.g., admissions, timetables, clubs, exams]
Tone: [Friendly and informal / Professional / Bilingual]
What it should NOT do: [e.g., give medical advice, access personal records]
```

### Step 2 — Write the System Prompt (45 min)
The system prompt is the hidden instruction that configures the AI's behaviour. Craft one for your campus chatbot:

**Template to start from:**
```
You are [Chatbot Name], a helpful and friendly AI assistant for [College Name].
Your role is to help students find information about [list topics].

Personality: [describe tone — friendly, professional, helpful]
Language: [English only / bilingual / regional language preference]

You have knowledge about:
- [Topic 1]: [brief description of what you know]
- [Topic 2]: [brief description]
- [Continue for each topic]

When you don't know something, say: "I don't have that information right now. 
Please contact [specific office/email] for help with this."

Never:
- Give medical, legal, or financial advice
- Share personal student information
- Make up facts about the college

Always:
- Be welcoming to new students
- Suggest the relevant department or contact if you can't answer
- Respond in the same language the student uses
```

Refine this system prompt through testing — iterate at least 3 times.

### Step 3 — Build the Knowledge Base (60 min)
Create a document with 20 realistic Q&A pairs covering your college.

**Categories to include (2-4 questions each):**
- Admissions and enrollment
- Academic calendar and timetables
- Exams and results
- Fees and payments
- Library and facilities
- Clubs and extracurriculars
- Placement and internships
- Support services (counselling, IT helpdesk)
- Campus facilities (canteen, transport, hostels)
- COVID/hybrid study policies

Format each entry as:
```
Q: [Student question, written naturally as a student would ask]
A: [Clear, concise answer — under 60 words]
Source: [Where this information comes from, e.g., college website, handbook]
```

### Step 4 — Test the Chatbot (60 min)
Test your chatbot system prompt with 15 conversation scenarios.

**Test categories:**
- 5 straightforward questions (should answer correctly)
- 3 ambiguous questions (tests clarification ability)
- 3 out-of-scope questions (tests boundary behaviour)
- 2 multi-turn conversations (tests context retention)
- 2 edge cases (odd phrasing, incomplete questions)

**For each test, document:**

| # | Test Query | Expected Response | Actual Response | Pass/Fail | Notes |
|---|-----------|-------------------|-----------------|-----------|-------|
| 1 | | | | | |

### Step 5 — Evaluation Report (45 min)
Write a 1-page evaluation covering:
1. Overall accuracy rate (how many of 15 tests passed?)
2. What types of questions it handled well
3. What types of questions it struggled with
4. Three specific improvements you would make to the system prompt
5. What a production version would need that this prototype lacks (e.g., real database access, authentication)

### Step 6 — Python Interface (Optional, 60 min)
Build a simple command-line interface for your chatbot:

```python
# Campus chatbot CLI interface
# Loads the system prompt from a file
# Takes user input in a loop
# Formats and displays responses
# Type 'quit' to exit
```

Use GitHub Copilot or ChatGPT to help build this in Python.

---

## Deliverables

- [ ] Chatbot definition document (Step 1)
- [ ] Final system prompt (after at least 3 iterations)
- [ ] Knowledge base (20 Q&A pairs)
- [ ] Test results table (15 tests)
- [ ] Evaluation report (1 page)
- [ ] (Optional) Python script
- [ ] Reflection: What makes a good chatbot? What would real users find frustrating?

---

## Extension Tasks

- Add the chatbot to a free platform like Poe.com or use the OpenAI Playground to make it shareable
- Conduct a user test with 3 classmates — ask them to use the chatbot and collect their feedback
- Design a conversation flow diagram showing how the chatbot handles different query paths
