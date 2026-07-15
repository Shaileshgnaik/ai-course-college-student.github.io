# Project: AI-Powered Learning Planner

**Difficulty:** Beginner to Intermediate
**Estimated time:** 4–5 hours
**Tools:** ChatGPT, Microsoft Copilot, optionally Excel or Notion

---

## Problem Statement

Students struggle to manage multiple subjects, assignments, exams, and personal commitments. Most planning tools are generic and don't adapt to individual learning styles or subject difficulty.

This project uses AI to build a personalised, adaptive learning planner tailored to one student's specific semester.

---

## What You'll Build

A complete AI-generated learning planning system:
1. A semester overview with all subjects, exams, and deadlines mapped
2. A weekly study schedule optimised for your learning style
3. Subject-specific study strategies for each of your courses
4. An exam preparation countdown plan
5. A wellbeing and productivity guide

---

## Step-by-Step Guide

### Step 1 — Capture Your Semester (20 min)
Fill in this semester snapshot:

```
Current semester: [e.g., Semester 3, July–November 2026]
Subjects (list all): 
  1. [Subject name] — [exam date] — [difficulty: easy/medium/hard]
  2. [Subject name] — [exam date] — [difficulty]
  3. [Continue for all subjects]
Upcoming assignments: [list with due dates]
Available study hours per day: [weekdays] [weekends]
Learning style: [Visual / Reading-writing / Hands-on / Listening]
Your biggest challenge: [e.g., procrastination, understanding theory, time management]
Extracurricular commitments: [clubs, jobs, sports — with time commitments]
```

### Step 2 — Generate Your Semester Overview (30 min)
```
I'm a [your year] year [your degree] student. Here is my semester snapshot:
[paste your snapshot]

Create a semester overview that:
1. Lists all subjects with their exam dates and estimated preparation time needed
2. Identifies the 3 highest-priority subjects based on difficulty and exam proximity
3. Maps out major milestones month by month
4. Flags any conflicts or crunch periods (multiple exams/deadlines close together)
5. Recommends how to distribute study time across subjects (percentages)
```

### Step 3 — Weekly Schedule Generator (45 min)
```
Create a detailed weekly study schedule for a [your degree] student with this semester:
[paste your subjects and hours available]

Requirements:
- Respect my available hours: [weekday hours] on weekdays, [weekend hours] on weekends
- Use time-blocking (assign specific subjects to specific time slots)
- Include: revision blocks, assignment work time, and buffer for unexpected tasks
- Apply spaced repetition: review harder subjects more frequently
- Include breaks using the Pomodoro technique (25 min study / 5 min break)
- Reserve Sunday evenings for weekly planning and review

Format as a table with days as columns and time slots as rows.
```

Evaluate the schedule: is it realistic? Adjust it to match your real life.

### Step 4 — Subject-Specific Study Strategies (45 min)
For each of your subjects, generate tailored strategies:
```
I'm studying [subject name] as part of [your degree].
My exam is on [date] and I currently find it [easy/medium/hard].
My learning style is [your style].

Create a subject-specific study strategy that includes:
1. Best approach for this type of subject (memorisation vs understanding vs practice)
2. Recommended study resources (types, not just generic suggestions)
3. Active recall techniques suited to this subject
4. How to structure a 2-hour study session for this subject
5. 3 common mistakes students make in this subject and how to avoid them
```

### Step 5 — Exam Countdown Plan (30 min)
For your most important upcoming exam:
```
My [subject] exam is on [date]. Today is [today's date]. I have [X days] to prepare.
My current confidence level is [1-10].
Topics to cover: [list your topics]
I can study [X hours] per day until the exam.

Create a day-by-day countdown study plan that:
- Covers all topics with appropriate depth
- Builds in revision days (not just first-pass learning)
- Gets progressively lighter in the final 2 days (consolidation, not cramming)
- Includes daily goals I can check off
- Ends with a "night before" checklist
```

### Step 6 — Wellbeing & Productivity Guide (20 min)
```
I'm a college student preparing for a busy exam period. 
Create a personalised wellbeing and productivity guide covering:
1. Sleep recommendations during exam season
2. Study environment optimisation
3. How to handle anxiety and overwhelm
4. Nutrition tips for focus and energy
5. How to maintain social connections without losing study time
6. Signs that I need to take a proper break
Keep it practical and realistic for a student budget and schedule.
```

---

## Deliverables

- [ ] Semester snapshot document (your input)
- [ ] Semester overview (priorities, milestones, time distribution)
- [ ] Weekly schedule (table format, edited to be realistic)
- [ ] Subject strategy guides (one per subject, minimum 3 subjects)
- [ ] Exam countdown plan for your next major exam
- [ ] Wellbeing guide
- [ ] Reflection: Did following the AI-generated plan actually help? What did you change?

---

## Extension Tasks

- Build the schedule in Excel or Google Sheets with conditional formatting to show completion
- Set up a weekly planning ritual: each Sunday, use AI to review the previous week and plan the next
- Ask AI to act as an accountability coach: *"I told you I would study 3 hours yesterday. I only did 1. Help me understand why and plan better for this week."*
- Create a semester retrospective at the end: *"Here was my plan vs what actually happened. What can I learn for next semester?"*
