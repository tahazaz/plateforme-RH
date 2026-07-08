# Functional Requirements

## Introduction

This document describes the main functional requirements of the HR Platform.

Functional requirements define what the system must do.

---

# FR-001 Authentication

The system must allow users to log in securely using email and password.

Users must be redirected to the correct dashboard according to their role:

- Employee
- Manager
- HR Administrator
- System Administrator

---

# FR-002 Role-Based Access

The system must restrict access to features based on the user's role.

Example:

- Employees access personal features.
- Managers access team features.
- HR accesses global HR features.
- Administrators access technical settings.

---

# FR-003 Employee Dashboard

The system must provide each employee with a personal dashboard including:

- Profile summary
- Leave balance
- Latest notifications
- Onboarding progress
- Recent documents

---

# FR-004 Manager Dashboard

The system must provide managers with a team dashboard including:

- Team members
- Pending leave requests
- Team calendar
- Onboarding progress
- Performance reviews

---

# FR-005 HR Dashboard

The system must provide HR users with a global dashboard including:

- Total employees
- Active contracts
- Leave statistics
- Onboarding status
- HR alerts
- Reports

---

# FR-006 Leave Management

The system must allow employees to:

- Submit leave requests
- View request status
- Cancel pending requests

The system must allow managers to:

- Approve leave requests
- Reject leave requests
- View team absences

The system must allow HR to:

- Configure leave rules
- View all leave requests
- Override leave decisions

---

# FR-007 Document Management

The system must allow HR to upload documents for employees.

Employees must be able to download their own documents.

Documents may include:

- Contracts
- Payslips
- Certificates
- HR letters
- Company policies

---

# FR-008 Onboarding

The system must generate an onboarding checklist for each new employee.

The onboarding module must allow:

- Task assignment
- Task validation
- Progress tracking
- Manager follow-up
- HR supervision

---

# FR-009 Performance Evaluation

The system must allow managers to create evaluations for employees.

Employees must be able to view their evaluations.

HR must be able to monitor evaluation campaigns.

---

# FR-010 Notifications

The system must send notifications for important events:

- Leave request submitted
- Leave request approved
- Leave request rejected
- New document uploaded
- Onboarding task assigned
- Evaluation created

---

# FR-011 AI Assistant

The system must provide an AI assistant able to:

- Answer HR questions
- Explain company policies
- Summarize documents
- Help employees during onboarding
- Assist HR with repetitive requests

---

# FR-012 Reporting

The system must provide reports for HR users.

Reports may include:

- Employee count
- Leave statistics
- Onboarding progress
- Turnover indicators
- Document status
- Performance evaluation progress
