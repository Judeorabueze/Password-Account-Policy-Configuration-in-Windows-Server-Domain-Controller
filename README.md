# Password & Account Policy Configuration in Windows Server Domain Controller

## Overview

In this project, I configured Password and Account Policies within a Windows Server Domain Controller (Active Directory environment) to enforce strong authentication standards and improve organizational security. This ensures that all domain users comply with best practices for password complexity and account protection.

## Objectives
- Implement password security best practices for domain users.
- Enforce account lockout policies to defend against brute-force login attempts.
- Gain hands-on experience with Active Directory and Group Policy Management.

## Technical Environment & Tools
- Windows Server 2019 (Domain Controller)
- Active Directory Domain Services (AD DS)
- Group Policy Management Console (GPMC)

## Target Password & Account Configurations

### Password Policy
- Minimum password length: 12 characters
- Password complexity: Enabled (uppercase, lowercase, numbers, special characters)
- Maximum password age: 90 days
- Minimum password age: 1 day
- Enforce password history: 5 previous passwords remembered

### Account Lockout Policy
- Account lockout threshold: 5 invalid attempts
- Account lockout duration: 30 minutes
- Reset account lockout counter after: 15 minutes

