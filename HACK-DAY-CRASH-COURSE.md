# Hack Day Crash Course — Open-Source AI

This is a short crash course for the Hacktoberfest Hack Day.

It is designed to help you understand the main concepts behind the challenge without going too deep into AI/ML theory.

You do **not** need to be an AI/ML expert.

---

# 1. What is Open Source?

Open-source software is software whose source code is publicly available under a license that allows others to use, modify, and share it.

A public GitHub repository is **not automatically open source**.

Your project should include an open-source license such as:

- MIT
- Apache-2.0
- GPL-3.0

Reference:
- https://choosealicense.com/
- https://opensource.org/licenses

---

# 2. What is Open-Weight AI?

An open-weight model is an AI model whose trained weights are available to use or run according to the model provider's terms.

Open-weight does **not always mean fully open source**, so always check the model's license or usage terms.

For this Hack Day, **Google Gemma** is the key partner technology.

---

# 3. What is an LLM?

LLM stands for **Large Language Model**.

An LLM can understand and generate text and, depending on the model, may also work with images, code, or other inputs.

A basic AI application often looks like:

```text
User
  ↓
Prompt
  ↓
Model
  ↓
Response
```

You do not need to train a model for the Hack Day.

You can use an existing model inside your application.

---

# 4. What is a Prompt?

A prompt is the instruction or information sent to an AI model.

Example:

```text
You are a code-review assistant.

Review the following JavaScript code and identify:
1. Bugs
2. Performance issues
3. Accessibility issues
```

A good prompt usually explains:

- What the model should do
- What information it has
- What output you expect
- Any rules it should follow

---

# 5. What is Context?

Context is the information you provide to the model so it can answer a question or perform a task correctly.

Example:

```text
User Question
+
Relevant Documentation
+
Instructions
↓
AI Model
↓
Answer
```

This is important because an AI model does not automatically know everything about your application or data.

---

# 6. What is RAG?

RAG stands for **Retrieval-Augmented Generation**.

Instead of asking an AI model to answer using only its existing knowledge, your application first retrieves useful information and gives it to the model.

Example:

```text
User Question
      ↓
Search / Retrieve Data
      ↓
Relevant Context
      ↓
AI Model
      ↓
Answer
```

RAG is commonly used for:

- Documentation assistants
- Knowledge search
- Research tools
- Support assistants

---

# 7. What are Embeddings?

Embeddings convert text or other information into numerical representations.

They make it easier to find information based on **meaning**, not only exact keywords.

Embeddings are commonly used in:

- Semantic search
- RAG
- Recommendation systems
- Document search

You only need to understand the basic idea.

---

# 8. What is an AI Agent?

A normal AI application may simply return an answer.

An AI agent can go further and use tools or perform actions.

Example:

```text
User
 ↓
AI Agent
 ↓
Decides what to do
 ↓
Uses a Tool
 ↓
Gets the Result
 ↓
Responds
```

An agent may use:

- APIs
- GitHub
- Databases
- Search
- Files
- Custom application functions

---

# 9. What is Tool Calling?

Tool calling allows an AI model to request that your application execute a function.

Example:

```text
User: "Get information from this GitHub repository."

AI Agent
   ↓
Calls GitHub API
   ↓
Gets repository data
   ↓
Analyses it
   ↓
Returns the result
```

This is one of the core concepts behind AI agents.

---

# 10. What is an Agent Skill?

An Agent Skill is a reusable set of instructions and supporting files that teaches an AI agent how to perform a task.

A skill can include:

```text
skill-name/
│
├── SKILL.md
├── scripts/
├── references/
└── assets/
```

A skill might teach an agent how to:

- Review React code
- Test APIs
- Analyse accessibility
- Review GitHub issues
- Generate documentation

Reference:
- https://agentskills.io/

---

# 11. What is a Model Harness?

A model harness is the software around an AI model.

The model is only one part of an AI application.

A harness may manage:

```text
Prompts
   ↓
Model
   ↓
Tools
   ↓
Memory
   ↓
Context
   ↓
Actions
```

It may handle:

- Prompts
- Tool execution
- Model selection
- Context
- Memory
- Responses
- Actions

For the Hack Day, you do not need to build a complex harness unless your project specifically focuses on one.

---

# Challenge Technology

The Hack Day has two challenges: Best Open-Source AI Project, which the concepts above cover, and Best Use of Gemma 4.

---

## 12. Google Gemma

Gemma is Google's family of lightweight, open-weight AI models.

For the MLH challenge, participants can build with **Gemma 4 through the Gemini API**.

Possible uses include:

- Text and image applications
- AI assistants
- Productivity tools
- Learning tools
- Community tools
- AI-powered developer tools

A simple architecture could look like:

```text
Frontend
   ↓
Backend
   ↓
Gemini API
   ↓
Gemma
   ↓
Response
```

For the Gemma challenge, the project should clearly identify the Gemma model being used and show the integration in the code or demo.

References:
- https://hacktoberfest-handbook.mlh.com/hack-days-partner-modules/partner-challenge-google-gemma
- https://mlh.link/gemma
- https://mlh.link/gemma-quickstart
- https://mlh.link/gemma-docs
- https://mlh.link/gemma-beginnerguide

---

# What Makes a Strong Hack Day Project?

A strong project should:

- Solve a clear problem
- Have a working demo
- Use open-source or open-weight AI meaningfully
- Show actual technical work by the team
- Be available in a public GitHub repository
- Include an open-source license
- Clearly mention the AI model or technology used
- Explain how the AI technology contributes to the project
- Include setup and run instructions

A simple README structure can be:

```text
Project Name

Problem

Solution

How It Works

Architecture

AI / Partner Technology Used

Setup Instructions

How to Run

Team Members

License
```

---

# Which Challenge Should You Choose?

Choose based on what you want to build.

### If you want to build with Gemma 4, especially on images, screenshots, or documents

Explore **Best Use of Gemma 4**.

### If you want to build with another open-source or open-weight model, an agent skill, or a model harness

Explore **Best Open-Source AI Project**.

---

# Final Reminder

You are not expected to become an expert before the event.

The goal is to understand enough that terms such as:

```text
Open Source
Open Weight
LLM
Prompt
Context
RAG
Embeddings
AI Agent
Tool Calling
Agent Skill
Model Harness
Gemma
```

do not feel completely new when the Hack Day begins.

---

## Must Read Before the Event

**Please go through this crash course before attending the Hack Day. This is a must so that you understand the core concepts and can focus on building during the event.**

All links shared in this file are provided only as **references**.

You are completely free to learn these topics from any source you prefer — official documentation, blogs, YouTube videos, courses, tutorials, or any other learning platform.

What matters is that you understand the concepts, not where you learn them from.
