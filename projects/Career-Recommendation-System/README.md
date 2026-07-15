---
layout: default
title: "Career Recommendation System"
permalink: /projects/career-recommendation/
---

# Project: Career Recommendation System

**Difficulty:** Intermediate
**Estimated time:** 4–6 hours
**Tools:** ChatGPT or Microsoft Copilot, optionally Python (Google Colab)

---

## Problem Statement

Many students don't know which AI-related career paths suit their skills, interests, and degree. Generic career advice doesn't account for individual strengths.

This project builds a structured career recommendation workflow using AI — a system that takes a student's profile as input and outputs personalised career guidance.

---

## What You'll Build

An AI-powered career guidance tool that:
1. Takes a student's skills, interests, and degree as input
2. Recommends 3 suitable AI-era career paths with reasoning
3. Maps skill gaps for each career path
4. Creates a personalised 6-month development roadmap
5. Generates a learning resource guide

---

## Step-by-Step Guide

### Step 1 — Build Your Student Profile (20 min)
Complete this profile for yourself (or a fictional student):

```
Name: [Your name]
Degree: [Your degree and year]
Technical skills: [List your tech skills, e.g., Python basics, Excel, SQL]
Soft skills: [e.g., communication, problem-solving, teamwork]
Interests: [What topics/industries interest you?]
Preferred work style: [Independent / collaborative / creative / analytical]
Career goal: [Any existing ideas, or "open to suggestions"]
Available learning time: [Hours per week you can dedicate to upskilling]
```

### Step 2 — Career Path Recommendation Prompt (30 min)
```
You are a career counsellor specialising in AI and technology careers.
Based on this student profile, recommend the top 3 AI-related career paths.
For each career path provide:
1. Career title and one-sentence description
2. Why it suits this student (based on their profile)
3. Typical starting salary range (India/global)
4. Day-to-day responsibilities
5. Key companies that hire for this role
6. One person to follow on LinkedIn in this field

Student profile: [paste your profile]
```

### Step 3 — Skill Gap Analysis (30 min)
For each recommended career (take the top recommendation):
```
I want to become a [career title]. My current skills are: [paste your skills].
Perform a skill gap analysis:
1. Skills I already have that are relevant
2. Skills I need to develop (ranked by priority)
3. Skills that are "nice to have" vs "essential"
4. Realistic timeline to bridge the gap (given [X hours/week])
```

### Step 4 — 6-Month Roadmap (30 min)
```
Create a detailed 6-month career development roadmap for someone who wants to 
become a [career title] starting from my current skill level: [your skills].
I have [X hours per week] for learning.

Month 1-2: Foundation building
Month 3-4: Core skill development  
Month 5-6: Portfolio and job preparation

For each month include: specific topics to learn, resources (free preferred), 
projects to build, and milestones to measure progress.
```

### Step 5 — Learning Resource Guide (30 min)
```
Create a curated learning resource guide for aspiring [career title]s.
Organise by category:
- Free online courses (with URLs)
- YouTube channels
- Books (beginner and advanced)
- Podcasts
- Communities and forums
- Certifications to pursue (with estimated cost and time)
Prioritise free and low-cost resources.
```

### Step 6 — Build a Simple Prompt-Based Recommender (Optional Python, 45 min)
If you want a technical challenge, build a simple Python script that:
- Asks the user for their skills and interests
- Formats the input into the recommendation prompt
- Calls the output prompt and displays a formatted result

Use this as your starting comment in VS Code/Colab and let GitHub Copilot help:
```python
# Simple career recommendation tool
# Prompts user for their degree, skills, and interests
# Formats the input and generates a career recommendation query
# Displays the top 3 career paths with key information
```

---

## Deliverables

- [ ] Your student profile document
- [ ] Career recommendation output (3 paths) with your evaluation
- [ ] Skill gap analysis for your top career choice
- [ ] 6-month roadmap (reviewed and personalised by you)
- [ ] Learning resource guide
- [ ] (Optional) Python script
- [ ] Reflection: How accurate was the AI? What would a human career counsellor add?

---

## Extension Tasks

- Run the same profile through 3 different AI tools and compare recommendations
- Conduct a mock interview for your top career using AI: *"Interview me for a junior [role] position. Ask one question at a time."*
- Find 3 real job listings for your top career and ask AI to score your profile against each listing
