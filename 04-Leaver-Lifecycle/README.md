# Leaver Lifecycle

## Overview

This section documents the secure offboarding of an employee from the Northwind Manufacturing Active Directory environment.

## Scenario

An approved HR termination request is received for an employee whose access must be revoked in accordance with company security and compliance policies.

## Tasks Performed

- Verified HR termination approval
- Captured the employee's existing identity attributes and access
- Disabled the Active Directory account
- Removed application, department, role, VPN, and licensing group memberships
- Retained **Domain Users** as the primary group
- Moved the account to the **Disabled Users** Organizational Unit
- Verified account status and OU placement using PowerShell
- Documented ServiceNow work notes
- Collected audit evidence before and after offboarding

## PowerShell Commands Used

```powershell
Get-ADUser noah.thompson -Properties Enabled |
Select Name,Enabled

Get-ADUser noah.thompson |
Select Name,DistinguishedName
```

## Offboarding Validation

PowerShell verification confirmed that:

- The account was successfully disabled.
- The identity object was preserved.
- The user was moved to the **Disabled Users** Organizational Unit.
- Application-specific security groups were removed.
- The **Domain Users** primary group remained intact.

## Technologies Used

- Active Directory Domain Services
- Windows PowerShell
- VMware Workstation
- ServiceNow workflow simulation

## IAM Best Practices Demonstrated

- Verified HR approval before processing termination.
- Applied least privilege by removing unnecessary access.
- Disabled the account immediately after termination.
- Preserved the identity object for auditing and compliance.
- Validated changes using PowerShell.
- Maintained complete audit evidence throughout the offboarding process.

## Evidence

This folder contains:

- Active Directory screenshots (before and after offboarding)
- PowerShell validation output
- User account disablement evidence
- Disabled Users OU verification
- ServiceNow termination workflow documentation
- Audit trail screenshots
