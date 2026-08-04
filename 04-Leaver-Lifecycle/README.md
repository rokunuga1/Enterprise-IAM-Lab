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
- # Leaver Lifecycle

## Overview
(Keep your existing content)

## Scenario
(Keep your existing content)

## Tasks Performed
(Keep your existing content)

## PowerShell Commands Used

```powershell
Get-ADUser noah.thompson -Properties Enabled |
Select Name,Enabled

Get-ADUser noah.thompson |
Select Name,DistinguishedName
```

## Evidence

- Screenshot – Noah Thompson account before offboarding
- Screenshot – Active Directory account disabled
- Screenshot – PowerShell verification (Enabled = False)
- Screenshot – User moved to Disabled Users OU

## Offboarding Validation

The employee account was successfully disabled and moved to the **Disabled Users** organizational unit.

PowerShell validation confirmed:

- Account disabled
- Identity preserved
- Organizational Unit updated
- Verified that no application-specific security groups were assigned to the employee at the time of offboarding.

## IAM Best Practices Demonstrated

- Verified HR termination approval before processing the request.
- Disabled the Active Directory account immediately upon termination.
- Verified the account status using PowerShell.
- Moved the user to the Disabled Users Organizational Unit.
- Preserved the identity object for audit and compliance purposes.
- Collected evidence to support the completed offboarding process.
- Evidence-based validation

## Evidence

Screenshots, PowerShell outputs, ServiceNow records, and audit documentation will be stored in this folder.
