# Business Rules

## Introduction

This document defines the business rules governing the HR Platform.

Business rules describe the constraints and behaviors that must always be respected by the system.

---

# Authentication

BR-001

A user must authenticate before accessing the platform.

---

BR-002

Each user has exactly one role.

Possible roles:

- Employee
- Manager
- HR Administrator
- System Administrator

---

BR-003

Only active users can access the platform.

---

BR-004

Passwords must be encrypted.

---

# User Management

BR-005

Only HR Administrators can create employee accounts.

---

BR-006

An employee belongs to one department.

---

BR-007

Each employee has one direct manager.

---

BR-008

An employee cannot modify sensitive HR information.

Examples:

- Salary
- Contract
- Position
- Department

---

# Leave Management

BR-009

Only employees can submit leave requests.

---

BR-010

A leave request must be validated by the employee's manager.

---

BR-011

HR may override a leave request if necessary.

---

BR-012

A leave request has one of the following statuses:

- Pending
- Approved
- Rejected
- Cancelled

---

BR-013

An employee may cancel a leave request only if it has not yet been approved.

---

# Documents

BR-014

Employees can only access their own documents.

---

BR-015

HR can upload, edit and delete HR documents.

---

BR-016

Managers cannot modify employee contracts.

---

# Onboarding

BR-017

Each new employee receives an onboarding checklist.

---

BR-018

The onboarding process starts automatically after account creation.

---

BR-019

Managers can monitor onboarding progress.

---

# Performance Evaluation

BR-020

Only managers can evaluate employees.

---

BR-021

Employees can view their own evaluations.

---

BR-022

HR can access all evaluations.

---

# Notifications

BR-023

Every important action generates a notification.

Examples:

- Leave approved
- New document
- New evaluation
- Contract updated

---

# Artificial Intelligence

BR-024

AI may assist users but never replace HR decisions.

---

BR-025

AI suggestions must always be validated by a human.

---

BR-026

AI cannot modify employee data automatically.

---

# Security

BR-027

Users may only access resources according to their role (RBAC).

---

BR-028

Every important action must be logged.

Examples:

- Login
- Account creation
- Leave approval
- Contract modification

---

BR-029

Sensitive documents must only be visible to authorized users.

---

BR-030

Inactive users cannot authenticate.

---

# General Rules

BR-031

Every employee has one unique identifier.

---

BR-032

Every leave request belongs to one employee.

---

BR-033

Every uploaded document belongs to one employee.

---

BR-034

Every notification belongs to one user.

---

BR-035

Every evaluation is created by one manager.
