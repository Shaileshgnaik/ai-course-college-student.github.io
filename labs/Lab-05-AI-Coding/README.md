---
layout: default
title: "Lab 05 - AI Coding"
permalink: /labs/lab-05/
---

# Lab 05 — AI Coding Assistant

**Duration:** 90 minutes
**Module:** Follows Module 07 — AI for Programming
**Tools needed:** VS Code with GitHub Copilot, OR ChatGPT/Copilot as a fallback
**Language:** Python (recommended); JavaScript alternative provided where applicable

---

## Objectives

By the end of this lab you will:
- Generate working Python code using AI prompts
- Debug broken code using an AI assistant
- Create a simple web page with AI assistance
- Understand the importance of reviewing AI-generated code

---

## Setup Check

Before starting, confirm:
- [ ] VS Code is open
- [ ] GitHub Copilot extension is installed and signed in
- [ ] Python is installed (`python --version` in terminal)
- [ ] Alternatively: Google Colab is open at colab.research.google.com

---

## Part 1: Generate Python Code from Comments (25 minutes)

**Task:** Write Python programs using only comments as instructions.

Create a new file `lab05_exercises.py` in VS Code.

**Exercise 1.1 — List operations**
Type this comment and let Copilot complete the code:
```python
# Function that takes a list of numbers and returns:
# - the average
# - the maximum value
# - the minimum value
# - count of numbers above the average
```

Run the function with `[12, 45, 7, 89, 23, 56, 34]` and verify the output is correct.

**Exercise 1.2 — String processing**
```python
# Function that takes a sentence and returns:
# - word count
# - character count (excluding spaces)
# - the longest word
# - the sentence reversed word by word
```

Test with: `"Artificial Intelligence is transforming every industry"`

**Exercise 1.3 — File handling**
```python
# Function that reads a CSV file with columns: name, score
# Returns the name of the student with the highest score
# If there are ties, return all tied names
```

Create a test CSV file manually with 5 student names and scores.

**For each exercise, document:**
- Did the AI generate working code on the first attempt?
- What did you have to fix or modify?

---

## Part 2: Debugging with AI (20 minutes)

The following Python scripts contain bugs. Copy each one and use an AI assistant to identify and fix the bugs.

**Buggy Script 1:**
```python
def calculate_average(numbers):
    total = 0
    for num in numbers:
        total = total + num
    average = total / len(numbers)
    return average

scores = [85, 92, 78, 96, 88]
print("Average score:", calcualte_average(scores))
print("Passing students:", sum(1 for s in scores if s > 90))
```

**Buggy Script 2:**
```python
students = {"Alice": 85, "Bob": 92, "Charlie": 78}

for name, score in students:
    if score >= 90:
        print(f"{name} passed with distinction")
    elif score >= 70:
        print(f"{name} passed")
    else:
        print(f"{name} needs improvement")
```

**For each bug:**
1. Describe the bug in plain English
2. Paste the code to your AI assistant with: *"Find and fix the bugs in this Python code. Explain each bug."*
3. Verify the fixed code runs correctly
4. Did you spot the bug before the AI?

---

## Part 3: Build a Simple Web Page with AI (25 minutes)

**Task:** Use AI to generate a simple HTML/CSS web page for a student portfolio.

**Step 1 — Generate the HTML structure:**
Ask ChatGPT or Copilot:
```
Create a simple, professional HTML and CSS student portfolio page for a 
final-year computer science student. Include:
- A header with name and tagline
- An "About Me" section (placeholder text)
- A "Skills" section with 6 AI-related skills
- A "Projects" section with 2 placeholder projects
- A contact section with email and GitHub links
Use inline CSS. Keep it clean and modern. No JavaScript needed.
```

**Step 2 — Save as `portfolio.html` and open in a browser**

**Step 3 — Customise:**
- Replace placeholder text with your actual name and details
- Ask AI to change the colour scheme: *"Update the CSS to use a dark blue and white colour scheme"*
- Ask AI to add a new section: *"Add a Certifications section after the Skills section"*

---

## Part 4: Code Documentation (20 minutes)

Take the code you wrote in Part 1 and ask AI to document it properly.

**Prompt:**
```
Add proper Python docstrings to each function in this code. 
Include: a one-line description, parameters with types, return value with type, and one usage example.
[paste your code]
```

Then ask AI to generate a README for your script:
```
Write a README.md for this Python script. Include: what it does, 
how to run it, example inputs and outputs, and any dependencies.
```

**Evaluate the documentation:**
- Is it accurate?
- Is it complete?
- Would a new developer understand what the code does from the docs alone?

---

## Lab Submission

Submit:
1. `lab05_exercises.py` with your three functions (Part 1) + notes on what you modified
2. Debugging worksheet: bug description, AI explanation, fixed code (Part 2)
3. `portfolio.html` — your customised portfolio page (Part 3)
4. Documented version of your code + generated README (Part 4)

**Grading criteria:**
- 3 working Python functions with documentation of AI assistance (4 marks)
- 2 bugs found and fixed with explanations (2 marks)
- Working portfolio HTML page (2 marks)
- Code documentation complete and accurate (2 marks)
