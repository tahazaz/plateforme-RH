# System Architecture

## Overview

The HR Platform follows a modern three-tier architecture composed of:

- Frontend
- Backend
- Database

Artificial Intelligence services are integrated as an independent component.

---

# Global Architecture

Employee
        │
Manager │
HR      │
Admin   │
        ▼

Frontend (React)

        │ REST API

Backend (Spring Boot)

        │

PostgreSQL Database

        │

AI Services (OpenAI / Local LLM)

---

# Frontend

Responsibilities:

- User Interface
- Authentication
- Dashboard
- Forms
- Notifications
- Charts
- AI Chat Interface

Technology:

- React
- TypeScript
- Material UI

---

# Backend

Responsibilities:

- Business Logic
- Security
- REST API
- Authentication
- Role Management
- Validation
- File Management

Technology:

- Spring Boot
- Spring Security
- JWT

---

# Database

Technology:

PostgreSQL

Main Entities:

- Employee
- Department
- Manager
- LeaveRequest
- Document
- Evaluation
- Notification
- User
- Role
- OnboardingTask

---

# Artificial Intelligence

Responsibilities:

- HR Chatbot
- Document Summarization
- Email Generation
- Recommendation Engine
- Smart Search
- Knowledge Base

---

# Security

Authentication:

- JWT

Authorization:

- RBAC (Role-Based Access Control)

Password Encryption:

- BCrypt

---

# File Storage

Documents:

- Contracts
- Payslips
- Certificates

Storage:

- Local Storage (development)
- AWS S3 / Azure Blob (production)

---

# API Communication

Frontend

↓

REST API

↓

Spring Boot

↓

Database

↓

AI Services

---

# Scalability

Future modules:

- Recruitment
- Payroll
- Time Tracking
- Expense Management
- Learning Management
- Mobile Application
