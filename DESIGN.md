@@ -0,0 +1,152 @@
# 🧩 OpenVista AI – Design Document

## 1. Overview

OpenVista AI is a failure-aware career and learning navigation platform designed to reduce dropouts and wrong career choices. It combines AI-driven learning roadmaps with real-world micro-internship simulations so users can understand difficulty levels and validate interest early.

---

## 2. Design Goals

* Highlight high-failure learning areas (Churn Zones)
* Provide simplified survival resources
* Simulate real job tasks in short sessions
* Keep system modular and scalable
* Ensure fast response and good UX

---

## 3. User Personas

### 3.1 Student / Beginner

* Unsure about career path
* Needs guidance and confidence

### 3.2 Career Switcher

* Wants to test a new field quickly
* Needs realistic job exposure

### 3.3 Educator / Mentor (Future)

* Wants insights into learner struggles

---

## 4. Functional Requirements

* User authentication
* Career selection
* Failure-aware roadmap generation
* Churn Zone display
* Micro-internship task generation
* Task submission
* AI feedback and scoring
* Progress tracking

---

## 5. Non-Functional Requirements

* Scalability
* Low latency
* Security
* Reliability
* Accessibility

---

## 6. High-Level Architecture

Frontend → API Gateway → Application Services → AI Layer → Data Layer

---

## 7. Component Design

### 7.1 Frontend

* React.js UI
* Code editor for tasks
* Roadmap visualization

### 7.2 Backend Services

* User Service
* Roadmap Service
* Churn Zone Engine
* Micro-Internship Engine
* Feedback Engine

### 7.3 AI Layer

* LLM for generation
* Embedding model
* RAG pipeline

### 7.4 Data Layer

* PostgreSQL (structured data)
* Vector DB (embeddings)
* Redis (cache)

---

## 8. Data Flow

1. User selects career
2. Backend requests roadmap
3. AI generates roadmap with churn zones
4. Data stored in DB
5. User explores and tries micro-internship
6. AI evaluates submission
7. Feedback returned to user

---

## 9. Database Design (High-Level)

Tables:

* users
* careers
* roadmaps
* churn_zones
* tasks
* submissions
* feedback

---

## 10. Security Design

* JWT authentication
* Input validation
* Role-based access (future)

---

## 11. UX Principles

* Simple and clean UI
* Minimal clicks
* Clear warnings for churn zones
* Encouraging language

---

## 12. Future Enhancements

* Multilingual support
* Mobile app
* Mentor matching
* Analytics dashboard

---

## 13. Design Philosophy

"Prepare users for reality, not just motivation."

PathPilot AI focuses on honesty, clarity, and practical experience.
