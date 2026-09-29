# 🎤 EventQ

### AI-Powered Audience Q&A Platform for Live Events

EventQ is a modern event engagement platform designed to make audience Q&A more organized, accessible, and intelligent.

It allows event organizers to create events and collect questions from their audience, including questions submitted through text and voice. EventQ also explores AI-powered processing to help organizers manage and understand audience questions more efficiently.

🔗 **Live Demo:** [Launch EventQ](https://event-q-web.vercel.app/)

🔒 **Source Code:** Private

---

## 📸 Screenshots
### EventQ Login
<img width="1860" height="956" alt="EventQ-login" src="https://github.com/user-attachments/assets/ff5d5ecf-cef7-4cac-bb73-7e408a0ba67d" />


### EventQ Dashboard
<img width="1850" height="944" alt="EventQ-dashboard" src="https://github.com/user-attachments/assets/4ba5723b-1532-4ad2-98af-40f0eb8ca68a" />


### Event Insights

<img width="1850" height="944" alt="EventQ-dashboard" src="https://github.com/user-attachments/assets/d3932aab-8b5c-40e1-a732-ec34a977a3d0" />


### Audience Questions



---

# ✨ Key Features

- 🎤 Create and manage events
- 👥 Audience participation through event-specific access
- ❓ Submit questions during live events
- 🎙️ Voice-based question submission
- 🌐 English and Hindi/Hinglish interaction
- 🤖 AI-assisted question processing
- 🔄 Question management and organization
- 🧩 Designed for handling large volumes of audience questions
- 📱 Responsive user interface
- 🔐 Authentication and protected application workflows
- ⚡ Modern full-stack architecture
- 🧪 End-to-end testing with Playwright
- 🚀 Production deployment through Vercel

---

# 🤖 AI Functionality

One of the main goals of EventQ is to explore how Generative AI can improve live-event audience interaction.

EventQ is designed to process audience questions using AI-based workflows.

### AI capabilities include:

- Understanding questions submitted in different languages
- Processing voice-based questions
- Converting spoken questions into usable text
- Helping normalize audience questions
- Identifying similar or duplicate questions
- Helping organizers organize large numbers of questions
- Supporting more efficient question management during live events

The AI layer is designed to reduce the manual effort required by event organizers when dealing with a large audience.

---

# 🏗️ Architecture

EventQ follows a modern full-stack architecture with a frontend application, backend services, database, AI integrations, authentication, testing, and deployment infrastructure.

### High-Level Architecture

![EventQ Architecture](architecture/architecture.png)

```text
                    ┌─────────────────────┐
                    │      Audience       │
                    │  Web / Mobile UI    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       EventQ        │
                    │    React Client     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │      API Layer      │
                    │       NestJS        │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
      ┌─────────────┐   ┌─────────────┐   ┌─────────────┐
      │   MongoDB   │   │ AI Services │   │    Auth     │
      │  Database   │   │    / LLM    │   │   & Users   │
      └─────────────┘   └─────────────┘   └─────────────┘
                               │
                               ▼
                       ┌───────────────┐
                       │ Voice / Speech│
                       │   Processing  │
                       └───────────────┘
