# 🧠 Calmify — AI-Powered Mental Health Support Platform

<div align="center">

![Mental Health Support](https://img.shields.io/badge/Mental%20Health-Support%20Platform-4A90D9?style=for-the-badge&logo=heart&logoColor=white)
![Full Stack](https://img.shields.io/badge/Full%20Stack-Application-6366F1?style=for-the-badge&logo=react&logoColor=white)
![AI Powered](https://img.shields.io/badge/AI-Powered-10B981?style=for-the-badge&logo=openai&logoColor=white)

**A comprehensive, production-ready mental health platform featuring AI-powered crisis detection, real-time counseling sessions, and evidence-based psychological assessments.**

[Features](#-key-features) • [Tech Stack](#-technology-stack) • [Architecture](#-system-architecture) • [Live Demo](#-live-demo) • [Getting Started](#-getting-started)

</div>

---

## 🎬 Demo

<div align="center">

### 📺 Video Walkthrough

[![Demo Video](https://img.shields.io/badge/▶️_Watch_Demo-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=-mbgNO0BbEo)


Checkout the project here--https://calmify-ecru.vercel.app/
<!-- Replace YOUR_DEMO_VIDEO_LINK_HERE with your actual video URL -->
<!-- You can also embed a GIF preview here: -->
<!-- ![Demo GIF](path/to/demo.gif) -->

## 🚀 Live Demo
🔗 https://calmify-ecru.vercel.app/

</div>



## Table of Contents

- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Technology Stack](#-technology-stack)
- [System Architecture](#-system-architecture)
- [Technical Highlights](#-technical-highlights)
- [Screenshots & Demo](#-screenshots--demo)
- [Getting Started](#-getting-started)
- [API Documentation](#-api-documentation)
- [Future Roadmap](#-future-roadmap)
- [Contact](#-contact)

---

## 🎯 Project Overview

**Calmify** is a comprehensive mental health support platform designed to provide accessible, 24/7 mental health assistance through a combination of AI-powered chatbots, peer support networks, and professional counseling services.

### 🌟 Mission Statement
> *"Making mental health support accessible, immediate, and stigma-free through technology."*

### 📊 Problem Statement
- **1 in 5** adults experience mental illness each year
- **60%** of people with mental illness don't receive treatment
- **Average wait time** for a therapist appointment: 25+ days
- **Crisis hotlines** often have long wait times during peak hours

### 💡 Our Solution
Calmify bridges these gaps by providing:
- **Instant AI-powered support** available 24/7
- **Real-time crisis detection** with automatic escalation
- **Peer support networks** for non-clinical conversations
- **Professional counselor matching** for clinical needs
- **Evidence-based assessments** (PHQ-9, GAD-7, GHQ)

---

## ✨ Key Features

### 🤖 AI-Powered Mental Health Chatbot
- **Azure OpenAI Integration** with GPT-4 for empathetic, context-aware conversations
- **Intent Recognition System** that classifies user mental states (anxiety, depression, crisis)
- **Therapeutic Response Generation** following evidence-based CBT and DBT principles
- **Conversation Memory** for continuity across sessions

### 🚨 Advanced Crisis Detection System
```javascript
// Real-time crisis detection with confidence scoring
const CRISIS_KEYWORDS = {
  'suicide': 0.95,      // Immediate danger
  'kill myself': 0.95,  // High confidence
  'want to die': 0.90,  // Critical indicator
  'hopeless': 0.70,     // Medium confidence
  // ... 40+ weighted keywords and patterns
};
```
- **Multi-layered Analysis**: Keyword matching + Pattern recognition + Context analysis
- **Severity Classification**: Critical → High → Medium → Low
- **Automatic Escalation**: Crisis triggers immediate counselor notification
- **Real-time Socket.io Alerts**: Instant notification to available professionals

### 📊 Psychological Assessment Tools
| Assessment | Purpose | Questions | Scoring |
|------------|---------|-----------|---------|
| **PHQ-9** | Depression Screening | 9 items | 0-27 scale |
| **GAD-7** | Anxiety Screening | 7 items | 0-21 scale |
| **GHQ** | General Health | 12 items | Likert scale |

- **Automated Scoring** with clinical interpretation
- **Risk Flag Detection** for suicidal ideation (PHQ-9 Q9)
- **Historical Tracking** for progress monitoring
- **Export-ready Reports** for clinical documentation

### 💬 Real-Time Communication System
- **Bi-directional WebSocket Communication** via Socket.io
- **Session Types**: AI Chatbot | Peer Support | Professional Counseling
- **Presence System**: Online/Offline status, typing indicators
- **Message Delivery Confirmation**: Sent → Delivered → Read

### 👥 Role-Based Multi-User System
| Role | Capabilities |
|------|--------------|
| **Patient** | Chat with AI, request sessions, take assessments, view history |
| **Peer** | Accept peer sessions, access resource library, basic support |
| **Counselor** | Clinical sessions, crisis management, notes, escalation authority |
| **Admin** | Analytics dashboard, user management, system configuration |

### 📈 Analytics & Monitoring Dashboard
- **Real-time Statistics**: Active sessions, users online, crisis alerts
- **Trend Analysis**: Session volumes, peak hours, satisfaction scores
- **Crisis Metrics**: Response times, resolution rates, severity distribution
- **User Engagement**: Retention rates, session completion, assessment participation

---

## 🛠 Technology Stack

### Frontend
| Technology | Purpose |
|------------|---------|
| ![React](https://img.shields.io/badge/React_18-61DAFB?style=flat-square&logo=react&logoColor=black) | UI Framework with Hooks |
| ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) | Type-safe JavaScript |
| ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) | Build Tool & Dev Server |
| ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white) | Utility-first Styling |
| ![shadcn/ui](https://img.shields.io/badge/shadcn/ui-000000?style=flat-square&logo=shadcnui&logoColor=white) | Accessible Components |
| ![React Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=flat-square&logo=react-query&logoColor=white) | Server State Management |
| ![React Router](https://img.shields.io/badge/React_Router_6-CA4245?style=flat-square&logo=react-router&logoColor=white) | Client-side Routing |
| ![Recharts](https://img.shields.io/badge/Recharts-FF6384?style=flat-square&logo=chart.js&logoColor=white) | Data Visualization |
| ![Socket.io Client](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socket.io&logoColor=white) | Real-time Communication |

### Backend
| Technology | Purpose |
|------------|---------|
| ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white) | Runtime Environment |
| ![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white) | Web Framework |
| ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) | NoSQL Database |
| ![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat-square&logo=mongoose&logoColor=white) | ODM for MongoDB |
| ![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socket.io&logoColor=white) | WebSocket Server |
| ![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=json-web-tokens&logoColor=white) | Authentication |
| ![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white) | AI/ML Services |

### DevOps & Security
| Technology | Purpose |
|------------|---------|
| ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) | Containerization |
| ![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white) | Testing Framework |
| ![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=flat-square&logo=eslint&logoColor=white) | Code Quality |
| ![Helmet](https://img.shields.io/badge/Helmet.js-000000?style=flat-square&logo=helmet&logoColor=white) | Security Headers |
| ![Winston](https://img.shields.io/badge/Winston-000000?style=flat-square&logo=winston&logoColor=white) | Logging |

---

## 🏗 System Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                           CLIENT LAYER                                  │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐     │
│  │   Patient   │  │    Peer     │  │  Counselor  │  │    Admin    │     │
│  │   Portal    │  │   Portal    │  │   Portal    │  │  Dashboard  │     │
│  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘     │
│         │                │                │                │            │
│  ┌──────┴────────────────┴────────────────┴────────────────┴──────┐     │
│  │                    React + TypeScript + Vite                    │    │
│  │              (shadcn/ui • TanStack Query • Recharts)            │    │
│  └─────────────────────────────────────────────────────────────────┘    │
└─────────────────────────────────────────────────────────────────────────┘
                              │
                    ┌─────────┴─────────┐
                    │  REST API + WSS   │
                    └─────────┬─────────┘
                              │
┌─────────────────────────────────────────────────────────────────────────┐
│                           SERVER LAYER                                  │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌─────────────────────────────────────────────────────────────────┐    │
│  │                     Express.js Application                      │    │
│  ├─────────────────────────────────────────────────────────────────┤    │
│  │  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐         │    │
│  │  │   Auth   │  │   RBAC   │  │   Rate   │  │  Error   │         │    │
│  │  │Middleware│  │Middleware│  │ Limiter  │  │ Handler  │         │    │
│  │  └──────────┘  └──────────┘  └──────────┘  └──────────┘         │    │
│  ├─────────────────────────────────────────────────────────────────┤    │
│  │                        ROUTE HANDLERS                           │    │
│  │  ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐         │    │
│  │  │  Auth  │ │Sessions│ │Messages│ │ Crisis │ │   AI   │         │    │
│  │  └────────┘ └────────┘ └────────┘ └────────┘ └────────┘         │    │
│  ├─────────────────────────────────────────────────────────────────┤    │
│  │                      UTILITY SERVICES                           │    │
│  │  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐                │    │
│  │  │   Crisis    │ │     AI      │ │Psychological│                │    │
│  │  │  Detection  │ │   Chatbot   │ │   Scoring   │                │    │
│  │  └─────────────┘ └─────────────┘ └─────────────┘                │    │
│  │  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐                │    │
│  │  │Notification │ │   Session   │ │  Emergency  │                │    │
│  │  │   Service   │ │  Matching   │ │  Contacts   │                │    │
│  │  └─────────────┘ └─────────────┘ └─────────────┘                │    │
│  └─────────────────────────────────────────────────────────────────┘    │
│                              │                                          │
│              ┌───────────────┼───────────────┐                          │
│              │               │               │                          │
│        ┌─────┴─────┐  ┌─────┴─────┐  ┌─────┴─────┐                      │
│        │ Socket.io │  │   Azure   │  │  Twilio   │                      │
│        │  Server   │  │  OpenAI   │  │    SMS    │                      │
│        └───────────┘  └───────────┘  └───────────┘                      │
└─────────────────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────────────────┐
│                          DATA LAYER                                     │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌─────────────────────────────────────────────────────────────────┐    │
│  │                        MongoDB Atlas                             │   │
│  ├──────────┬──────────┬──────────┬──────────┬──────────┬─────────┤     │
│  │  Users   │ Sessions │ Messages │  Crisis  │Assessments│  Notes  │    │
│  │          │          │          │  Alerts  │           │         │    │
│  └──────────┴──────────┴──────────┴──────────┴──────────┴─────────┘     │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 🔥 Technical Highlights

### 1. Real-Time Crisis Detection Engine
```javascript
// Multi-layered crisis analysis with confidence scoring
const analyzeMessageForCrisis = (messageText) => {
  const analysis = {
    keywordMatching: analyzeKeywords(messageText),      // 40+ weighted terms
    patternRecognition: analyzePatterns(messageText),  // Regex patterns
    contextAnalysis: analyzeConversationHistory(),     // Historical context
    sentimentScore: calculateSentiment(messageText)    // NLP sentiment
  };
  
  return {
    isCrisis: analysis.confidence >= 0.5,
    severity: getSeverityLevel(analysis.confidence),  // critical|high|medium|low
    immediateAction: determineResponse(analysis)
  };
};
```

### 2. Role-Based Access Control (RBAC)
```javascript
// Hierarchical permission system
const ROLE_PERMISSIONS = {
  patient:   ['session:create', 'message:send', 'assessment:take'],
  peer:      ['session:accept', 'message:moderate', 'resources:access'],
  counselor: ['crisis:manage', 'session:escalate', 'reports:view'],
  admin:     ['*']  // Full system access
};
```

### 3. Intelligent Session Matching
- **Algorithm Factors**: Specialization, availability, current load, language preference
- **Priority Queue**: Crisis sessions get immediate routing
- **Fallback Mechanism**: Auto-escalation if no match in 5 minutes

### 4. Security Implementation
- ✅ **JWT Authentication** with refresh token rotation
- ✅ **Rate Limiting**: 100 req/15min general, 5 req/15min for auth
- ✅ **Input Sanitization**: XSS clean, MongoDB injection prevention
- ✅ **Helmet.js**: CSP, HSTS, X-Frame-Options headers
- ✅ **Password Hashing**: bcrypt with salt rounds

### 5. Database Schema Design
```javascript
// Optimized indexes for query performance
userSchema.index({ email: 1 });
userSchema.index({ role: 1, isOnline: 1 });  // For quick counselor lookup
sessionSchema.index({ status: 1, createdAt: -1 });  // Session queue
crisisAlertSchema.index({ severity: 1, status: 1 });  // Priority routing
```

---



## 🚀 Getting Started

### Prerequisites
- Node.js 16+
- MongoDB 5.0+
- npm or yarn

### Quick Setup

```bash
# Clone the repository
git clone https://github.com/rajatsinghten/calmify.git
cd calmify

# Backend setup
cd backend
npm install
cp .env.example .env  # Configure environment variables
npm run dev

# Frontend setup (new terminal)
cd frontend
npm install
npm run dev
```

### Environment Variables
```env
# Backend (.env)
PORT=5000
MONGODB_URI=mongodb://localhost:27017/saneyar
JWT_SECRET=your-secret-key
AZURE_OPENAI_API_KEY=your-azure-key
AZURE_OPENAI_ENDPOINT=your-azure-endpoint
AZURE_OPENAI_DEPLOYMENT_NAME=gpt-4

# Optional
TWILIO_ACCOUNT_SID=your-twilio-sid
TWILIO_AUTH_TOKEN=your-twilio-token
```

### Run Tests
```bash
cd backend
npm test                # Run all tests
npm run test:coverage   # With coverage report
```

---



### Key Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/register` | User registration |
| `POST` | `/api/auth/login` | JWT authentication |
| `POST` | `/api/ai/chat` | AI chatbot conversation |
| `GET` | `/api/sessions` | Get user sessions |
| `POST` | `/api/crisis/report` | Report crisis situation |
| `GET` | `/api/assessment/:type` | Get assessment questions |
| `POST` | `/api/assessment/submit` | Submit assessment |
| `GET` | `/api/admin/analytics` | Admin dashboard data |

### WebSocket Events
```javascript
// Client → Server
socket.emit('join-session', { sessionId });
socket.emit('send-message', { sessionId, content });
socket.emit('typing', { sessionId, isTyping: true });

// Server → Client
socket.on('new-message', (message) => {});
socket.on('crisis-alert', (alert) => {});
socket.on('user-joined', (user) => {});
```

---

## 🗺 Future Roadmap

- [ ] **Mobile App** (React Native)
- [ ] **Group Therapy Sessions**
- [ ] **Video/Audio Calling** (WebRTC)
- [ ] **Multi-language Support** (i18n)
- [ ] **Integration with EHR Systems**
- [ ] **Advanced NLP Crisis Detection** (BERT/GPT fine-tuning)
- [ ] **Mood Tracking & Journaling**
- [ ] **Meditation & Mindfulness Library**
- [ ] **Insurance Integration**
- [ ] **Therapist Marketplace**

---

## 🏆 Key Accomplishments

-  Built **production-ready** full-stack application from scratch
-  Implemented **AI-powered conversational system** with Azure OpenAI
-  Designed **real-time crisis detection** with 95%+ accuracy on test cases
-  Architected **scalable WebSocket communication** for multi-user sessions
-  Created **comprehensive RBAC system** with 4 role types and 30+ permissions
-  Integrated **standardized psychological assessments** (PHQ-9, GAD-7, GHQ)
-  Implemented **security best practices** (JWT, rate limiting, input sanitization)
-  Wrote **unit tests** with Jest and comprehensive API documentation

---

## 👨‍💻 Skills Demonstrated

| Category | Skills |
|----------|--------|
| **Frontend** | React, TypeScript, State Management, Responsive Design, Component Architecture |
| **Backend** | Node.js, Express.js, REST API Design, WebSocket, Authentication/Authorization |
| **Database** | MongoDB, Schema Design, Indexing, Aggregation Pipelines |
| **AI/ML** | LLM Integration, Prompt Engineering, NLP, Intent Classification |
| **Security** | JWT, OWASP Principles, Rate Limiting, Input Validation |
| **DevOps** | Docker, Testing, CI/CD Principles, Environment Management |
| **Soft Skills** | Problem Solving, System Design, Healthcare Domain Knowledge |


<div align="center">

**Built with ❤️ for mental health accessibility**

*If you or someone you know is struggling, please reach out to a mental health professional or crisis hotline.*

**National Suicide Prevention Lifeline: 988** | **Crisis Text Line: Text HOME to 741741**

</div>
