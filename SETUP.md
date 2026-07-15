---
layout: default
title: Setup Guide
permalink: /setup/
---

# Environment Setup Guide

Complete this setup **before your first session**. All tools have a free tier suitable for this course.

---

## Step 1: Microsoft Account & Copilot

### Microsoft Account
1. Go to https://account.microsoft.com
2. Click **Create a Microsoft account** if you don't have one
3. Use your college email if possible (unlocks additional benefits)

### Microsoft Copilot (Free)
1. Go to https://copilot.microsoft.com
2. Sign in with your Microsoft account
3. Test it: type "Explain AI in simple terms" — you should get a response
4. **Note:** Microsoft 365 Copilot (in Word/Excel/PowerPoint) requires a licensed Microsoft 365 subscription. Check with your college IT team — many colleges provide free access for students.

---

## Step 2: ChatGPT

1. Go to https://chat.openai.com
2. Click **Sign up** and create a free account
3. The free tier (GPT-4o mini) is sufficient for all course exercises
4. Test it: type "What is machine learning?" to confirm it works

---

## Step 3: GitHub Account & GitHub Copilot (Free for Students)

### GitHub Account
1. Go to https://github.com
2. Click **Sign up** — use your college email
3. Verify your email address

### GitHub Student Developer Pack (Free GitHub Copilot)
1. Go to https://education.github.com/pack
2. Click **Get student benefits**
3. Verify your student status with your college email or student ID
4. Once approved, you get **GitHub Copilot for free** (usually approved within 1-3 days)

### GitHub Copilot in VS Code
1. Install VS Code: https://code.visualstudio.com
2. Open VS Code → Extensions (Ctrl+Shift+X / Cmd+Shift+X)
3. Search for **GitHub Copilot** → Install
4. Sign in with your GitHub account when prompted

---

## Step 4: Visual Studio Code

1. Download from https://code.visualstudio.com
2. Install the following extensions (search in Extensions panel):
   - **GitHub Copilot** — AI coding assistant
   - **Python** (by Microsoft) — Python language support
   - **Jupyter** — run Jupyter notebooks in VS Code
   - **Prettier** — code formatting

---

## Step 5: Python & Google Colab

### Option A: Google Colab (No installation required — recommended)
1. Go to https://colab.research.google.com
2. Sign in with a Google account
3. Click **New notebook** to confirm it works
4. Colab gives you free GPU access for ML exercises

### Option B: Local Python Installation
1. Download Python 3.10+ from https://python.org/downloads
2. During installation, check **Add Python to PATH**
3. Verify: open a terminal and run `python --version`
4. Install Jupyter: `pip install jupyter`

---

## Step 6: Kaggle Account (for Datasets & ML Exercises)

1. Go to https://kaggle.com
2. Click **Register** — free account
3. Go to **Learn** → confirm you can access the Intro to ML course
4. Optionally download the Kaggle CLI for dataset access: `pip install kaggle`

---

## Step 7: Hugging Face Account (for Module 04 & Beyond)

1. Go to https://huggingface.co
2. Click **Sign Up** — free account
3. Explore the **Models** tab — you'll use this in Modules 03 and 04

---

## Quick-Check Checklist

Before your first session, confirm each of these works:

- [ ] Microsoft Copilot — can have a conversation at copilot.microsoft.com
- [ ] ChatGPT — can send a message at chat.openai.com
- [ ] GitHub account created and email verified
- [ ] VS Code installed with GitHub Copilot extension
- [ ] Google Colab — can open a new notebook
- [ ] Kaggle account active
- [ ] Hugging Face account active

---

## Troubleshooting

| Problem | Solution |
|---------|---------|
| GitHub Copilot not activating | Ensure student pack is approved; sign out and back in to VS Code |
| Microsoft 365 Copilot unavailable | Use copilot.microsoft.com (free) as an alternative during labs |
| Google Colab slow | Switch runtime: Runtime → Change runtime type → T4 GPU |
| Python not found in terminal | Re-run installer and check "Add to PATH"; restart terminal |
| ChatGPT "at capacity" | Try Microsoft Copilot or Google Gemini (gemini.google.com) as alternatives |

---

## Need Help?

Raise your hand during the session or open an issue on the course GitHub repo:
https://github.com/Shaileshgnaik/ai-course-college-student.github.io/issues
