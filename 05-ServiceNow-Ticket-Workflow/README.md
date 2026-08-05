# ServiceNow IAM Workflow Simulation

## Overview

This section demonstrates a simulated Identity and Access Management (IAM) workflow using a ServiceNow-style process. The workflow follows enterprise IAM procedures for Joiner, Mover, and Leaver identity lifecycle events.

Although ServiceNow was not connected to this lab, the workflow mirrors how an IAM Analyst would receive, validate, process, document, and close identity requests in a production environment.

> **Note:** This workflow was simulated for portfolio purposes. ServiceNow was used to model enterprise IAM request management and approval processes. Active Directory and PowerShell tasks were performed in the lab environment to mirror production IAM operations.

---

# Workflow

```
HR Request
      │
      ▼
Manager Approval
      │
      ▼
ServiceNow Ticket Created
      │
      ▼
IAM Validation
      │
      ▼
Active Directory Changes
      │
      ▼
PowerShell Verification
      │
      ▼
Evidence Collection
      │
      ▼
Ticket Closed
```

---

# Joiner Workflow

## Request

New employee onboarding request received from Human Resources.

Employee:

Amina Bello

Employee ID:

E-10482

Department:

Finance

Manager:

Jordan Lee

---

## Validation

Completed:

- HR approval verified
- Manager approval verified
- Employee ID verified
- Duplicate account check completed

---

## IAM Actions

Performed:

- Created Active Directory user
- Assigned Employee ID
- Configured department
- Configured title
- Assigned Organizational Unit
- Assigned Microsoft 365 license group
- Assigned Finance security groups
- Assigned application groups

---

## Verification

Completed using:

- Active Directory Users and Computers
- PowerShell

Evidence collected.

Ticket closed.

---

# Mover Workflow

## Request

Employee transfer approved.

Employee:

Emily Thompson

Employee ID:

E-10040

Transfer:

Sales → Finance

---

## Validation

Verified:

- HR approval
- Manager approval
- Transfer effective date

---

## IAM Actions

Updated:

- Department
- Job Title
- Manager

Granted:

- Finance Role Group

Removed:

- Sales access

---

## Verification

Completed using:

- Active Directory
- PowerShell

Evidence collected.

Ticket closed.

---

# Leaver Workflow

## Request

HR termination request approved.

Employee:

Noah Thompson

Employee ID:

E-10024

---

## Validation

Verified:

- HR approval
- Employee identity
- Manager authorization

---

## IAM Actions

Performed:

- Disabled Active Directory account
- Verified account status
- Verified no application-specific security groups were assigned
- Moved user to Disabled Users OU

---

## Verification

Completed using:

- Active Directory
- PowerShell

Evidence collected.

Ticket closed.

---

# IAM Controls Demonstrated

- Least Privilege
- Role-Based Access Control (RBAC)
- Identity Governance
- Access Certification
- Separation of Duties
- Joiner-Mover-Leaver Lifecycle
- Active Directory Administration
- PowerShell Verification
- Change Documentation
- Audit Readiness

---

# Technologies Used

- Active Directory Domain Services
- Windows Server
- PowerShell
- VMware Workstation
- GitHub
- ServiceNow (Workflow Simulation)

---

# Skills Demonstrated

- Identity Lifecycle Management
- User Provisioning
- User Deprovisioning
- Active Directory Administration
- Organizational Unit Management
- Security Group Administration
- RBAC
- PowerShell
- Identity Verification
- Audit Documentation
- Technical Documentation
- GitHub Version Control
