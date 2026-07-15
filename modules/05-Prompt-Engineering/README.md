---
layout: default
title: "05 - Prompt Engineering"
permalink: /modules/05-prompt-engineering/
---

# Module 05 — Prompt Engineering

## Learning Objectives

By the end of this module students will:

- Understand what prompt engineering is and why it matters
- Apply core prompting techniques: zero-shot, few-shot, chain-of-thought
- Design effective prompts for different tasks (writing, coding, analysis)
- Build and maintain a personal prompt library

---

## Topics Covered

### 1. What is Prompt Engineering?

A prompt is any input you send to an AI model. Prompt engineering is the practice of designing and refining those inputs to get better, more accurate, and more useful outputs. Since LLMs are sensitive to how questions are framed, the same underlying request can produce dramatically different results depending on how it is worded.

Prompt engineering is not about tricks or hacks — it is about being precise, providing context, and communicating clearly with a system that is very good at following specific instructions but struggles with ambiguity.

### 2. Anatomy of a Good Prompt

The most effective prompts typically include five elements:

| Element | Purpose | Example |
|---------|---------|---------|
| **Role** | Sets the AI's expertise and perspective | "You are a career counsellor..." |
| **Task** | The specific action you want | "...write 3 interview tips..." |
| **Context** | Background information the AI needs | "...for a final-year CS student applying for internships..." |
| **Format** | How you want the output structured | "...as a numbered list..." |
| **Constraints** | Length, tone, or content boundaries | "...under 20 words each, professional tone." |

Not every prompt needs all five elements — simple tasks need less; complex tasks need more.

### 3. Zero-Shot, One-Shot, and Few-Shot Prompting

**Zero-shot:** Ask the AI to perform a task with no examples. Relies entirely on the model's pre-trained knowledge. Best for simple, well-defined tasks.

*Example: "Classify this sentence as Positive, Negative, or Neutral: 'The lecture was long but informative.'"*

**One-shot:** Provide one example before your actual request. Helps the model understand the expected format or style.

**Few-shot:** Provide 2–5 examples. Significantly improves accuracy on tasks with specific output formats or patterns. The examples act as "demonstrations" that guide the model's behaviour.

*Use few-shot when:* the output needs a specific format, classification is nuanced, or the task is unusual enough that zero-shot produces inconsistent results.

### 4. Chain-of-Thought Prompting

Chain-of-thought (CoT) prompting asks the AI to reason step-by-step before giving a final answer. This dramatically improves performance on tasks requiring multi-step reasoning — maths problems, logical analysis, planning.

**Standard prompt:** "A student has 5 assignments, each taking 2 hours. They have 8 free hours before the deadline. Can they finish?"

**Chain-of-thought prompt:** Same question, but add: "Think through this step by step before giving your answer."

The model will show its working rather than jumping to a conclusion, making errors easier to spot and the reasoning process visible.

### 5. Role Prompting and Persona Techniques

Assigning the AI a role ("You are a senior software engineer", "You are a Socratic tutor") changes the tone, vocabulary, depth, and approach of its responses. A response from "an expert in X" tends to be more specific and technically accurate than a generic response.

Role prompting is particularly effective for:
- Technical explanations (assign domain expertise)
- Writing in a specific style (assign a professional persona)
- Critical feedback (assign a "devil's advocate" or "reviewer" role)
- Structured tasks (assign a methodology: "Use the STAR method")

### 6. Iterative Prompting and Refinement

Rarely does the first prompt produce the ideal output. Expert prompt engineers treat prompting as an iterative process: send a prompt, evaluate the response, identify what is missing or wrong, and refine the prompt accordingly.

Common refinement moves:
- Add specificity: "Make the second point more concrete, with a real example"
- Constrain format: "Rewrite this as bullet points, max 15 words each"
- Adjust tone: "Make this more formal / casual / technical"
- Redirect: "Focus more on the risks, less on the benefits"
- Expand: "Go deeper on point 3"

### 7. Prompt Patterns for Common Tasks

**Summarisation:** "Summarise the following text in [X] bullet points, each under [Y] words, for an audience of [Z]: [text]"

**Explanation:** "Explain [concept] to a [audience level] student who has no background in [field]. Use an analogy. Keep it under 150 words."

**Code generation:** "Write a Python function that [description]. Include: input parameters with types, a docstring, and one usage example."

**Feedback/review:** "Review the following [essay/code/plan] as a [role]. Identify: the 2 strongest aspects and the 3 most important improvements. Be specific and constructive."

**Decision support:** "I need to choose between [Option A] and [Option B] for [purpose]. Compare them across: [criteria 1], [criteria 2], [criteria 3]. Present as a table, then give a recommendation."

### 8. Evaluating and Comparing Prompt Outputs

Not all AI outputs are equal. Develop the habit of evaluating responses against these criteria:
- **Accuracy:** Is the information correct? Can you verify key claims?
- **Relevance:** Does it actually address what you asked?
- **Completeness:** Did it cover all parts of the prompt?
- **Format compliance:** Did it follow your formatting instructions?
- **Tone:** Is the register appropriate for your intended use?
- **Usability:** Can you use this output directly, or does it need significant editing?

---

## Demonstrations

- Live iterative prompt refinement — from vague to precise in 4 steps
- Chain-of-thought for a logic and planning problem
- Role prompting comparison: generic vs. expert persona on the same request

## Hands-on Activities

- Rewrite 5 weak prompts into effective ones (use the 5-element framework)
- Build a 10-prompt library for your area of study
- Use chain-of-thought to solve a multi-step problem with an LLM

## Assignment

Create a "Prompt Engineering Cheat Sheet" for your discipline — a reference document a classmate could use immediately. See `../../assessments/assignments/README.md` for full brief.

## Additional Resources

- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [Learn Prompting (free, open-source)](https://learnprompting.org/)
- [Anthropic Prompt Library](https://docs.anthropic.com/en/prompt-library/library)

---

*Previous: [Module 04 — Generative AI & LLMs](../04-Generative-AI-and-LLMs/README.md)  |  Next: [Module 06 — Microsoft Copilot](../06-Microsoft-Copilot/README.md)*
