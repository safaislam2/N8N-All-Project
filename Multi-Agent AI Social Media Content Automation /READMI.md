# 🤖 Multi-Agent AI Social Media Content Automation

An AI-powered social media content automation workflow built with **n8n** and multiple specialized AI agents.

This workflow takes a simple topic and post type from a Google Form, generates professional content, creates an image-generation prompt, generates a visual, prepares the LinkedIn post, and sends a notification to Slack.

---

## 🚀 Project Overview

The main goal of this project is to automate the social media content creation process using a **Multi-Agent AI Architecture**.

Instead of asking one AI agent to perform every task, the workflow uses multiple specialized agents. Each agent has a specific responsibility.

### Workflow

```text
Google Form
     ↓
Description Generator Agent
     ↓
Image Prompt Generator Agent
     ↓
Title Generator Agent
     ↓
AI Image Generation
     ↓
LinkedIn Post
     ↓
Slack Notification
```

---

## 🧠 Multi-Agent Architecture

### 1. Description Generator Agent

The first AI agent receives the topic and post type from the Google Form.

It analyzes the information and generates a professional social media content description.

**Input:**

* Post Topic
* Post Type

**Output:**

* Professional content description

---

### 2. Image Prompt Generator Agent

The second AI agent takes the generated content and creates a detailed image-generation prompt.

The prompt is designed to produce a professional visual that matches the topic and content.

**Input:**

* Generated content
* Topic

**Output:**

* Detailed image-generation prompt

---

### 3. Title Generator Agent

The third AI agent creates an engaging and professional title based on the generated content.

**Input:**

* Topic
* Generated description

**Output:**

* Professional post title

---

## 🎨 AI Image Generation

After the image prompt is generated, the workflow uses an HTTP Request/API to generate a visual automatically.

This removes the need to manually create an image for every social media post.

The generated visual can then be used with the social media content.

---

## 💼 LinkedIn Integration

The workflow includes a LinkedIn step for preparing/publishing the generated content.

The LinkedIn integration can use the generated:

* Title
* Description
* Image

to create a professional social media post.

> **Note:** LinkedIn OAuth authentication must be configured before the final LinkedIn publishing step can be executed.

---

## 🔔 Slack Notification

After the automation reaches the Slack step, a notification is automatically sent to the selected Slack channel.

Example:

```text
New social media content has been generated successfully.
```

This allows the workflow owner to monitor the automation without constantly opening n8n.

---

## 🛠️ Technology Stack

* n8n
* AI Agents
* Google Forms
* Google Gemini
* HTTP Request
* Image Generation API
* LinkedIn
* Slack

---

## ✨ Key Features

* ✅ Google Form based content input
* ✅ Multi-Agent AI architecture
* ✅ Automated content generation
* ✅ Automated title generation
* ✅ Automated image prompt generation
* ✅ AI image generation
* ✅ LinkedIn integration
* ✅ Slack notification
* ✅ Modular workflow structure
* ✅ Easy to extend
* ✅ Reduced manual content creation

---

## 🔄 How It Works

### Step 1 — Submit Content Information

The user submits a topic and post type through Google Forms.

Example:

```text
Post Topic:
How Multi-Agent AI Automation Can Transform Social Media Content Creation

Post Type:
Educational
```

### Step 2 — Generate Content

The Description Generator Agent analyzes the topic and creates professional content.

### Step 3 — Generate Image Prompt

The Image Prompt Generator Agent converts the content into a detailed visual-generation prompt.

### Step 4 — Generate Title

The Title Generator Agent creates an engaging title for the post.

### Step 5 — Generate Image

The HTTP Request node sends the generated image prompt to the configured image-generation API.

### Step 6 — LinkedIn

The generated content and visual are prepared for LinkedIn publishing.

### Step 7 — Slack

The workflow sends an automated Slack notification after the content-generation process.

---

## 🎯 Why Multi-Agent AI?

A single AI agent can perform multiple tasks, but separating the workflow into specialized agents provides better control and flexibility.

For example:

```text
Agent 1 → Content Generation
Agent 2 → Visual Prompt Generation
Agent 3 → Title Generation
```

Each agent can be improved independently.

This makes the workflow more modular, maintainable, and scalable.

---

## 📈 Potential Use Cases

This automation can be used for:

* Personal branding
* LinkedIn content creation
* Business marketing
* AI automation agencies
* Social media management
* Digital marketing
* Startup content creation
* Educational content
* Professional thought leadership

---

## 🔮 Future Improvements

Planned improvements include:

* [ ] Complete LinkedIn OAuth setup
* [ ] Automatic hashtag generation
* [ ] AI content quality checker
* [ ] Brand voice agent
* [ ] Human approval system
* [ ] Facebook integration
* [ ] Instagram integration
* [ ] X/Twitter integration
* [ ] Automatic content scheduling
* [ ] Google Sheets/Airtable database
* [ ] Error handling and retry system
* [ ] Social media analytics
* [ ] Performance tracking

---

## 📊 Example Input

```text
Topic:
How Multi-Agent AI Automation Can Transform Social Media Content Creation

Post Type:
Educational
```

### Expected Workflow Output

```text
Topic
   ↓
AI Description
   ↓
Professional Title
   ↓
Image Generation Prompt
   ↓
AI Generated Image
   ↓
LinkedIn Content
   ↓
Slack Notification
```

---

## 🎓 Learning Objectives

This project demonstrates practical implementation of:

* AI Agents
* Multi-Agent workflows
* Workflow automation
* API integration
* Social media automation
* AI image generation
* Slack integration
* LinkedIn integration
* n8n workflow orchestration

---

## 🚀 Future Vision

The long-term goal is to transform this workflow into a complete **AI Social Media Content Factory**.

The system can eventually research a topic, generate content, create branded visuals, validate the content, request approval, publish across multiple platforms, and track performance automatically.

---

## 👨‍💻 Project

**Project Type:** AI Automation / Multi-Agent System

**Built With:** n8n + AI Agents + APIs

**Primary Goal:** Automate professional social media content creation from a simple topic.

---

## ⭐ If You Like This Project

Feel free to explore the workflow, improve the agents, add new integrations, and extend the automation for other social media platforms.
