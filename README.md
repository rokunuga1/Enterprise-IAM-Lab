# Enterprise Identity and Access Management Lab

## Project Overview

This repository documents a simulated enterprise Identity and Access Management environment built for Northwind Manufacturing.

The lab demonstrates complete Joiner, Mover, and Leaver identity lifecycle workflows using Active Directory, PowerShell, role-based access control, and simulated ServiceNow request management.

## Business Scenario

Northwind Manufacturing requires standardized identity lifecycle processes to ensure employees receive appropriate access when hired, access is modified when job responsibilities change, and access is revoked promptly when employment ends.

The lab was designed to demonstrate how an IAM Analyst receives approved requests, performs identity administration, validates changes, documents work, and maintains audit evidence.

## Technologies Used

- Windows Server 2022
- Active Directory Domain Services
- Active Directory Users and Computers
- Windows PowerShell
- VMware Workstation
- Role-Based Access Control
- Simulated ServiceNow workflows
- Microsoft 365 licensing groups
- VPN and application access groups

## Repository Sections

### [01 — Environment Setup](./01-Environment-Setup)

Documents the Windows Server, Active Directory domain, static IP configuration, organizational units, security groups, and enterprise user structure.

### [02 — Joiner Lifecycle](./02-Joiner-Lifecycle)

Demonstrates onboarding a new employee, configuring identity attributes, assigning role-based access, and validating the completed provisioning.

### [03 — Mover Lifecycle](./03-Mover-Lifecycle)

Demonstrates transferring an employee between departments, changing identity attributes, removing obsolete access, assigning new access, and validating the completed changes.

### [04 — Leaver Lifecycle](./04-Leaver-Lifecycle)

Demonstrates employee offboarding, account disablement, access removal, license removal, movement to the Disabled Users OU, and post-offboarding validation.

### [05 — ServiceNow Ticket Workflow](./05-ServiceNow-Ticket-Workflow)

Contains simulated ServiceNow requests, approvals, IAM task execution, work notes, audit history, and ticket closure evidence.

## IAM Skills Demonstrated

- Joiner, Mover, and Leaver lifecycle administration
- Active Directory user provisioning and deprovisioning
- Organizational Unit administration
- Identity attribute management
- Security and distribution group management
- Role-Based Access Control
- Least-privilege access administration
- PowerShell identity validation
- Microsoft 365 license-group administration
- VPN and application-access management
- ServiceNow request and approval workflows
- Audit evidence collection
- IAM ticket documentation
- Access revocation and account disablement

## Lifecycle Summary

| Lifecycle | Scenario | Result |
|---|---|---|
| Joiner | New employee onboarding | Account created and authorized access assigned |
| Mover | Department transfer | Attributes and access updated for the new role |
| Leaver | Employee termination | Account disabled and access revoked |

## Important Disclaimer

This is a personal lab environment created for training and portfolio demonstration.

The ServiceNow interfaces and workflow records are simulations designed to represent enterprise request, approval, implementation, and audit processes. No production systems or real employee information were used.

## Author

**Rilwan Okunuga**

Identity and Access Management Portfolio Project
