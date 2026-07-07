# Database Design

## Overview

The database stores all information related to users, roles, departments, employees, leave requests, documents, onboarding, evaluations, notifications and AI interactions.

---

# Main Entities

## 1. User

Represents a person who can log in to the platform.

Attributes:

- id
- firstName
- lastName
- email
- passwordHash
- phone
- status
- createdAt
- updatedAt

Relationships:

- One user has one role.
- One user may belong to one department.
- One user may have one manager.

---

## 2. Role

Represents the access level of a user.

Attributes:

- id
- name
- description

Examples:

- Employee
- Manager
- HR
- Administrator

Relationships:

- One role can be assigned to many users.

---

## 3. Department

Represents a company department.

Attributes:

- id
- name
- description

Relationships:

- One department has many users.
- One department may have one manager.

---

## 4. EmployeeProfile

Stores HR information related to an employee.

Attributes:

- id
- userId
- jobTitle
- contractType
- hireDate
- salary
- emergencyContact
- address

Relationships:

- One employee profile belongs to one user.

---

## 5. LeaveRequest

Represents a leave or absence request.

Attributes:

- id
- employeeId
- managerId
- startDate
- endDate
- type
- reason
- status
- createdAt
- updatedAt

Status values:

- Pending
- Approved
- Rejected
- Cancelled

Relationships:

- One leave request belongs to one employee.
- One leave request is reviewed by one manager.

---

## 6. Document

Represents an HR document uploaded to the platform.

Attributes:

- id
- employeeId
- uploadedBy
- title
- fileName
- fileUrl
- category
- uploadDate

Categories:

- Contract
- Payslip
- Certificate
- Handbook
- Policy
- Other

Relationships:

- One document belongs to one employee.
- One document is uploaded by one HR user.

---

## 7. OnboardingTask

Represents a task assigned to a new employee.

Attributes:

- id
- employeeId
- title
- description
- status
- dueDate
- createdAt

Status values:

- To Do
- In Progress
- Done

Relationships:

- One onboarding task belongs to one employee.

---

## 8. Evaluation

Represents a performance review.

Attributes:

- id
- employeeId
- managerId
- title
- score
- comments
- evaluationDate
- createdAt

Relationships:

- One evaluation belongs to one employee.
- One evaluation is created by one manager.

---

## 9. Notification

Represents a notification sent to a user.

Attributes:

- id
- userId
- title
- message
- type
- isRead
- createdAt

Relationships:

- One notification belongs to one user.

---

## 10. AIConversation

Stores interactions with the AI assistant.

Attributes:

- id
- userId
- prompt
- response
- createdAt

Relationships:

- One AI conversation belongs to one user.

---

# Database Relationships Summary

- Role 1 ---- * User
- Department 1 ---- * User
- User 1 ---- 1 EmployeeProfile
- User 1 ---- * LeaveRequest
- User 1 ---- * Document
- User 1 ---- * OnboardingTask
- User 1 ---- * Evaluation
- User 1 ---- * Notification
- User 1 ---- * AIConversation

---

# First Version Tables

For the first version of the platform, the minimum required tables are:

- users
- roles
- departments
- employee_profiles
- leave_requests
- documents
- onboarding_tasks
- evaluations
- notifications
- ai_conversations
