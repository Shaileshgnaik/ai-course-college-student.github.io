# Module 07 — AI for Programming

## Learning Objectives

By the end of this module students will:

- Use GitHub Copilot to accelerate coding in VS Code
- Generate, explain, and debug code using AI assistants
- Apply AI to Python and JavaScript development workflows
- Understand the limits and risks of AI-generated code

---

## Topics Covered

### 1. AI Coding Assistants Overview

AI coding assistants use LLMs trained on billions of lines of code to help developers write, understand, and fix software. They work by completing code based on context — your file contents, comments, and the code you've written so far. Unlike traditional autocomplete, they can generate entire functions, suggest architectural patterns, explain unfamiliar code, and translate between programming languages.

The major tools in this space:
- **GitHub Copilot:** Deeply integrated into VS Code and other IDEs. The industry standard. Free for verified students via GitHub Education.
- **Cursor:** An AI-native code editor built on VS Code with deeper Copilot-style integration.
- **Replit AI:** In-browser coding with AI assistance. Good for beginners.
- **ChatGPT / Claude:** Not IDE-integrated, but excellent for explaining code, debugging, and generating standalone scripts.

### 2. GitHub Copilot — Setup and Features

GitHub Copilot integrates directly into VS Code as an extension. Once installed, it provides:

**Inline completions:** As you type, Copilot suggests completions in grey text. Press Tab to accept, Esc to dismiss.

**Copilot Chat (sidebar):** Ask questions about your code, request refactors, explain errors, and generate new code from natural language descriptions.

**Comment-to-code:** Write a comment describing what a function should do; Copilot generates the implementation.

**Ghost text:** When you start typing a function signature, Copilot predicts and completes the entire function body.

The most important habit: **always read AI-generated code before accepting it**. Copilot can be confidently wrong — especially for edge cases, security-sensitive operations, and domain-specific logic.

### 3. Generating Code from Comments and Prompts

The most effective way to use Copilot for code generation is via precise comments:

```python
# Function that validates an email address using regex
# Returns True if valid, False otherwise
# Handles edge cases: empty string, no @ symbol, no domain
```

Copilot will generate a complete implementation. The more specific your comment, the better the code. Think of comments as prompts — apply the same precision as you would in prompt engineering.

For larger tasks, use Copilot Chat with a detailed description: "Write a Python class for a simple bank account with methods for deposit, withdrawal, and balance checking. Include input validation and raise appropriate exceptions."

### 4. AI Code Explanation and Debugging

**Code explanation:** Paste any unfamiliar code into Copilot Chat and ask "Explain this code line by line" or "What does this function do and when would you use it?" This is one of the most valuable uses of AI for learning — you can understand code from open-source projects, legacy codebases, or tutorials far faster.

**Debugging:** Paste an error message and the relevant code. Ask: "I'm getting this error. What is causing it and how do I fix it?" Copilot typically identifies the issue and suggests a fix. For complex bugs, provide more context: "This function is supposed to return X but is returning Y when the input is Z."

**Code review:** Ask Copilot to review your code for common issues: "Review this function for security vulnerabilities, edge cases, and Python best practices."

### 5. Python with AI — Scripts, Data Analysis, Automation

Python is the dominant language for AI-assisted programming because of its readability and the richness of its library ecosystem. Common AI-assisted Python workflows:

**Data analysis:** Describe what you want to analyse; Copilot generates pandas/matplotlib code. "Read sales.csv, calculate monthly totals, and plot a line chart."

**Automation:** Describe a repetitive task; Copilot generates a script. "Script that renames all .jpg files in a folder to include today's date."

**API integration:** "Write Python code to fetch weather data from the OpenWeatherMap API and display the forecast for a given city."

**Web scraping:** "Scrape the titles and prices of products from [page structure description] using BeautifulSoup."

### 6. JavaScript with AI — Web Apps and UI

JavaScript is the language of the web. AI accelerates frontend development by generating HTML/CSS layouts, JavaScript logic, and React components from descriptions.

**HTML/CSS generation:** "Create a responsive navigation bar with a logo on the left and 4 menu items on the right. Use CSS flexbox."

**JavaScript logic:** "Write a function that validates a form — checks that all required fields are filled and the email contains an @ symbol."

**API calls:** "Write a fetch() call that gets posts from JSONPlaceholder and displays titles in an unordered list."

### 7. GitHub Copilot — Advanced Usage

Beyond basic completions, Copilot supports:
- **Test generation:** "Write unit tests for this function covering: normal case, empty input, and invalid type."
- **Documentation:** "Add JSDoc comments to this JavaScript function."
- **Refactoring:** "Refactor this function to use async/await instead of callbacks."
- **Language translation:** "Convert this Python function to JavaScript."

### 8. When Not to Trust AI-Generated Code

AI coding assistants are powerful but not reliable for:
- **Security-sensitive code:** Authentication, cryptography, input sanitisation — always have these reviewed by a security-aware developer
- **Complex algorithms:** AI may produce plausible-looking but subtly incorrect implementations of sorting, graph, or dynamic programming algorithms
- **Domain-specific logic:** AI has no knowledge of your business rules, database schemas, or system constraints
- **Cutting-edge libraries:** Copilot's training has a knowledge cutoff; new library versions may have breaking changes the model doesn't know about

The mindset: AI writes the boilerplate; you own the logic. Never ship code you don't understand.

---

## Demonstrations

- Generate a Python data analysis script from a plain English comment
- Build a simple JavaScript web app using AI prompts in VS Code
- Debug a broken function using Copilot Chat, then run the fixed code

## Hands-on Activities

- Use GitHub Copilot to complete 5 coding exercises from comment-only prompts
- Take a broken Python script and fix it using an AI assistant
- Build a mini HTML portfolio page using JavaScript with Copilot assistance

## Assignment

Build a small Python project of your choice using AI assistance. Document which parts were AI-generated and what you modified. See `../../assessments/assignments/README.md` for full brief.

## Additional Resources

- [GitHub Copilot Docs](https://docs.github.com/en/copilot)
- [GitHub Student Developer Pack](https://education.github.com/pack)
- [Replit AI](https://replit.com/)

---

*Previous: [Module 06 — Microsoft Copilot](../06-Microsoft-Copilot/README.md)  |  Next: [Module 08 — Responsible AI](../08-Responsible-AI/README.md)*
