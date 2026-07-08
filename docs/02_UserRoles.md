# User Roles

## Introduction

The HR Platform is designed around three main user roles. Each role has different responsibilities, permissions, and access to specific functionalities.

The goal is to ensure security, simplify navigation, and provide each user with the tools required for their daily tasks.

---

# 1. Employee

## Description

The employee is the primary user of the platform.

They can manage their personal HR activities, access company information, and interact with their manager and the HR department.

## Main Responsibilities

- View personal profile
- Access HR documents
- Request leave
- Follow onboarding tasks
- Read company policies
- Update personal information
- View notifications
- Contact HR

## Permissions

Can:

- View personal information
- Edit some personal information
- Download personal documents
- Submit leave requests
- Track request status
- View assigned tasks
- Receive notifications

Cannot:

- Access other employees' data
- Validate requests
- Modify company settings
- Manage users

---

# 2. Manager

## Description

Managers supervise one or several employees.

They are responsible for validating requests, monitoring performance, and ensuring team organization.

## Main Responsibilities

- Manage team members
- Approve leave requests
- Monitor employee performance
- Conduct performance reviews
- Assign objectives
- Follow onboarding progress

## Permissions

Can:

- View team information
- Approve or reject leave requests
- Create performance reviews
- Assign objectives
- View team dashboards
- Receive management alerts

Cannot:

- Modify HR policies
- Create new users
- Access confidential HR administration settings

---

# 3. Human Resources (HR)

## Description

The HR department manages the entire HR process and administers the platform.

HR users have the highest functional permissions.

## Main Responsibilities

- Employee management
- Contract management
- Recruitment
- Document management
- Leave policies
- Onboarding
- Company handbook
- Reporting

## Permissions

Can:

- Create employees
- Update employee records
- Delete or archive employees
- Upload HR documents
- Configure leave policies
- Manage company policies
- Generate reports
- Manage user roles
- Access dashboards
- Configure platform settings

---

# Access Matrix

| Feature | Employee | Manager | HR |
|----------|----------|----------|----|
| View personal profile | ✅ | ✅ | ✅ |
| Edit personal profile | ✅ | ✅ | ✅ |
| Request leave | ✅ | ❌ | ✅ |
| Approve leave | ❌ | ✅ | ✅ |
| View team | ❌ | ✅ | ✅ |
| Manage employees | ❌ | ❌ | ✅ |
| Manage contracts | ❌ | ❌ | ✅ |
| Upload documents | ❌ | ❌ | ✅ |
| Performance reviews | View only | Manage | Manage |
| Dashboard | Personal | Team | Global |
| Manage users | ❌ | ❌ | ✅ |
| Platform configuration | ❌ | ❌ | ✅ |

---

# Security Principle

The platform follows a **Role-Based Access Control (RBAC)** model.

Each authenticated user receives permissions according to their assigned role.

This approach ensures:

- Data confidentiality
- Secure access
- Separation of responsibilities
- Simplified maintenance
- Scalability for future roles

---

# Future Roles

The platform has been designed to easily support additional roles in the future, such as:

- Recruiter
- IT Administrator
- Finance Department
- External Consultant
- Intern
