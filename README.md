# 24SolveSphere
A digital platform where universities and industries can post real world problems and collaboratively source student-driven solutions
# SolveSphere 🌍

### Find a problem. Build a team. Create an impact.

SolveSphere is a student-first platform that connects students with real-world problems posted by communities, organizations, and individuals.

Instead of students starting with the question *"What project should I build?"*, SolveSphere starts with an actual problem that needs to be solved.

Students can discover challenges, understand the required skills, find teammates with complementary skills, build solutions, and track their impact.

---

## 🎯 Problem

Students often want practical, real-world project experience but face challenges such as:

- Finding meaningful problems to work on
- Understanding what skills a project requires
- Finding teammates with complementary skills
- Organizing project tasks and progress
- Measuring the impact of their work

At the same time, communities, organizations, and individuals face real-world problems but may not always have the technical teams or resources to build solutions.

SolveSphere aims to connect these two sides.

---

## 💡 Our Solution

SolveSphere provides a complete journey from a real-world problem to a student-built solution:

**Discover → Understand → Connect → Build → Measure**

### 1. Discover
Students can explore challenges based on issues, skills, and interests.

### 2. Understand
Each challenge provides information such as:

- Problem description
- Objectives
- Required skills
- Difficulty
- Potential impact

### 3. Connect
Students can:

- Create a team space
- Explore existing teams
- Find students with complementary skills
- Request to join teams
- Accept or reject team requests

### 4. Build
Teams can:

- Propose a solution
- Work on tasks
- Assign tasks to teammates
- Set deadlines
- Track project progress

### 5. Measure
Teams can track their impact through metrics such as:

- People reached
- Community hours
- Projects completed
- Outcomes achieved

---

## 🤖 AI-Powered Features

SolveSphere is designed to use AI at important points in the project journey.

### Skill Gap Analysis

Students can select their existing skills and compare them with the skills required by a challenge.

The system identifies:

- Matched skills
- Missing skills
- Why a missing skill matters
- A learning roadmap to help the student get started

### Planned AI Capabilities

The platform is designed to support additional AI features such as:

- Problem analysis and structuring
- AI-based team matching
- Duplicate challenge detection
- Similar solution detection
- Personalized skill development

> **Hackathon Prototype Note:** The current Skill Gap Analysis demonstration uses browser-based deterministic logic. A live AI provider integration is planned for the next version.

---

## 🖥️ Key Features

- 🔎 Challenge discovery and filtering
- 📋 Challenge details and requirements
- 🧠 Skill Gap Analysis
- 👥 Team creation and team discovery
- 🤝 Team join requests
- 🚀 Project workspace
- ✅ Task management
- 📊 Project progress tracking
- 🌍 Impact Snapshot
- 💾 Local persistence using LocalStorage
- 🔁 Duplicate detection concept
- 📱 Responsive web interface

---

## 🛠️ Technology Stack

Frontend:
- React
- TypeScript
- Vite
- Tailwind CSS
- Lucide Icons
- Wouter

Backend:
- Express.js

Storage:
- Browser LocalStorage

Current Prototype:
The current version is intentionally lightweight and does not require a database or external API keys to run.

---
Architecture:


                 ┌─────────────────────┐
                 │      User           │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   React Frontend    │
                 │                     │
                 │ Challenges          │
                 │ Teams               │
                 │ Skill Gap           │
                 │ Projects & Tasks    │
                 │ Impact Snapshot     │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Express Backend   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Future Services   │
                 │                     │
                 │ PostgreSQL          │
                 │ Authentication      │
                 │ AI API              │
                 │ Challenge Analysis  │
                 └─────────────────────┘
