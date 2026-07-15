---
layout: default
title: "04 - Generative AI & LLMs"
permalink: /modules/04-genai/
---

# Module 04 — Generative AI and Large Language Models

## Learning Objectives

By the end of this module students will:

- Understand what Generative AI is and how it differs from traditional AI
- Explain how Large Language Models (LLMs) work
- Identify popular foundation models and their capabilities
- Evaluate AI-generated outputs critically

---

## Topics Covered

### 1. Introduction to Generative AI

Generative AI refers to AI systems that can create new content — text, images, audio, video, and code — rather than simply classifying or predicting based on existing data. The outputs are not retrieved from a database; they are generated fresh each time, based on patterns learned during training. This is the breakthrough that has made AI visible and relevant to everyone, not just technical specialists.

### 2. Traditional AI vs Generative AI

Traditional AI systems are primarily **discriminative** — they learn to classify or predict. A spam filter decides if an email is spam or not. A recommendation engine predicts what you'll click. These systems answer "what is this?" or "what will happen?"

Generative AI systems answer "what should come next?" or "what would this look like?" They produce new content rather than categorising existing content. This distinction is why GenAI has unlocked entirely new categories of application — writing assistants, code generation, synthetic media, creative tools.

### 3. Large Language Models — How They Work

LLMs are neural networks (specifically Transformers) trained on massive text datasets — books, websites, code, scientific papers. Through training, they learn statistical patterns: which words tend to follow which other words, in what contexts, across millions of different topics.

At inference time (when you send a prompt), the model doesn't retrieve an answer — it **generates** one, token by token, predicting the most likely next token given everything that came before. Temperature controls how random these predictions are: low temperature = more predictable, high temperature = more creative.

This is why LLMs can discuss any topic fluently, but also why they can confidently produce false information — they are predicting plausible text, not retrieving verified facts.

### 4. Tokens, Context Windows, and Temperature

**Token:** The basic processing unit of an LLM. Roughly 1 token ≈ 0.75 words. "Machine learning" = 3 tokens. Models have a maximum number of tokens they can process in one interaction.

**Context window:** The total tokens the model can "see" at once — both your input and its output count toward this limit. GPT-4 has a 128,000 token context window. Claude supports up to 200,000. Larger context windows allow longer documents, more complex instructions, and multi-turn conversations.

**Temperature:** Controls output randomness. Temperature 0 = always chooses the most likely token (predictable, factual). Temperature 1+ = introduces more randomness (creative, varied, but more prone to errors). For factual tasks, use low temperature. For creative tasks, use higher temperature.

### 5. Popular Foundation Models (GPT-4, Claude, Gemini, Llama)

**GPT-4 / GPT-4o (OpenAI):** Powers ChatGPT and Microsoft Copilot. Multimodal (text + images). Strong coding and reasoning capabilities.

**Claude (Anthropic):** Known for long context windows (up to 200k tokens), safety-focused design, and strong document analysis. Accessible via claude.ai.

**Gemini (Google):** Deeply integrated with Google products. Strong at web search integration and multimodal tasks.

**Llama (Meta):** Open-source foundation models that anyone can run locally or fine-tune. Enables a broad ecosystem of customised AI applications.

**Mistral:** European open-source models known for efficiency — strong performance relative to model size.

### 6. Text, Image, Audio, and Video Generation

Modern GenAI spans modalities beyond text:
- **Image generation:** DALL-E 3, Stable Diffusion, Midjourney, Adobe Firefly. Generate images from text descriptions.
- **Audio generation:** ElevenLabs (voice cloning and text-to-speech), Suno (music generation).
- **Video generation:** Sora (OpenAI), Runway, Pika. Generate short videos from text prompts.
- **Code generation:** GitHub Copilot, Replit AI, Cursor. Generate, complete, and explain code.

**Multimodal models** can understand and generate across multiple types of content — GPT-4o can accept text and images as input and respond in text.

### 7. Hallucinations and AI Limitations

AI hallucinations occur when a model generates factually incorrect information presented with apparent confidence. They happen because the model is predicting plausible text, not retrieving facts. Common patterns include: inventing citations, describing events that didn't happen, attributing quotes to wrong people, and fabricating statistics.

**How to handle hallucinations:**
- Always verify important facts from AI output using authoritative sources
- Ask the AI to cite its sources and then check them
- Use lower temperature for factual tasks
- Prefer AI tools with web search access (Perplexity, Bing Copilot) for current information

Other limitations: knowledge cutoff dates, context window limits, inability to access real-time data (without tools), difficulty with precise arithmetic, and susceptibility to leading prompts.

### 8. Hands-on Demonstration

In this module you will directly compare multiple LLMs, observe a hallucination being generated, and generate content across modalities — building an empirical, critical understanding of what these tools can and cannot do.

---

## Demonstrations

- Text generation: blog post, email, code — same prompt, three different models
- Image generation with DALL-E or Copilot Designer
- Deliberately inducing and identifying a hallucination

## Hands-on Activities

- Prompt the same question to three different LLMs and compare responses
- Identify a hallucination in AI output and fact-check it using a search engine
- Generate a study guide for one of your subjects using an LLM, then verify 3 factual claims

## Assignment

Create an AI-powered study assistant using Copilot or ChatGPT. Document your prompts and evaluate the quality and accuracy of outputs. See `../../assessments/assignments/README.md` for full brief.

## Additional Resources

- [Andrej Karpathy — Intro to LLMs (YouTube)](https://www.youtube.com/watch?v=zjkBMFhNj_g)
- [Hugging Face — Open LLMs](https://huggingface.co/models)
- [OpenAI Documentation](https://platform.openai.com/docs)

---

*Previous: [Module 03 — Deep Learning & Neural Networks](../03-Deep-Learning-Neural-Networks/README.md)  |  Next: [Module 05 — Prompt Engineering](../05-Prompt-Engineering/README.md)*
