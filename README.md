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

## Implementation Steps

### 1. Configuring Password Policy in Windows Domain Controller
#### Steps Performed:

<b>a. Launch the Domain Controller VM</b>
- Opened the Domain Controller Virtual Machine and navigated to the <b>Server Manager</b> Dashboard.
- Clicked on <b>Tools</b> and selected <b>Group Policy Management</b>.

(See Pix 1)

<b>b. Access the Default Domain Policy</b>
- In the Group Policy Management Console, expanded:
<b>Forest: judeorabueze.com > Domains > judeorabueze.com > Group Policy Objects</b>.
- Located and selected the <b>Default Domain Policy</b>.

(See Pix 2)

<b>c. Open Group Policy Management Editor</b>
- Right-clicked on Default Domain Policy and selected Edit.
- Navigated to:
<b>Policies > Windows Settings > Security Settings > Account Policies > Password Policy</b>.

(See Pix 3)

Review and Update Password Policy Settings

Viewed the existing (default) password policy configuration.

Right-clicked each policy setting, selected Properties, and updated them as follows:

Minimum Password Length: Increased from 7 → 12 characters.

Maximum Password Age: Increased from 42 days → 90 days.

Enforce Password History: Reduced from 10 → 5 previous passwords remembered.

(See Pix 4 for updated configuration)






