# Mover Lifecycle

## Overview

This section documents an employee transfer between departments while maintaining identity continuity and enforcing least-privilege access.

---

## Scenario

Employee Emily Thompson transfers from Sales to Finance.

The IAM Administrator receives an approved HR transfer request and updates the employee identity according to corporate access policies.

---

## Tasks Performed

- Verified HR approval
- Updated Department attribute
- Updated Job Title
- Updated Manager
- Moved user to Finance OU
- Removed Sales security groups
- Added Finance security groups
- Assigned Finance role
- Verified membership with PowerShell
- Validated audit trail

---

## Technologies

- Active Directory Domain Services
- PowerShell
- VMware
- ServiceNow (Simulated)

---

## Evidence

Screenshots, PowerShell verification, ServiceNow ticket, and audit notes are stored in this folder.
