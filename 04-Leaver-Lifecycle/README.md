# Leaver Lifecycle

## Overview

This section documents the secure offboarding of an employee from the Northwind Manufacturing Active Directory environment.

## Scenario

An approved HR termination request is received for an employee whose access must be revoked according to company security policy.

## Tasks Performed

- Verified HR termination approval
- Captured the employee's existing access
- Disabled the Active Directory account
- Removed application, department, role, VPN, and licensing groups
- Retained Domain Users as the primary group
- Moved the account to the Disabled Users OU
- Verified account status and OU placement using PowerShell
- Documented ServiceNow work notes
- Created audit evidence and before-versus-after access records

## Technologies

- Active Directory Domain Services
- Windows PowerShell
- VMware Workstation
- ServiceNow workflow simulation

## IAM Principles Demonstrated

- Immediate access revocation
- Least privilege
- Identity lifecycle management
- Auditability
- Separation of duties
- Evidence-based validation

## Evidence

Screenshots, PowerShell outputs, ServiceNow records, and audit documentation will be stored in this folder.
