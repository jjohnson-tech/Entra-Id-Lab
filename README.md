# Entra-Id-Lab
Hands-on Microsoft Entra ID lab covering user creation, role assignment, security group management, Conditional Access, app registration, and sign-in log auditing in a Microsoft 365 tenant.

## Overview
Using the Microsoft Entra ID admin center connected to my existing Microsoft 365 tenant, this lab simulates core identity and access management tasks performed in real enterprise IT environments. The lab covers user creation, role assignment, security group management, Conditional Access policy review, application registration, and sign-in log auditing — reflecting the day-to-day responsibilities of IAM Analysts, Junior Sysadmins, and helpdesk teams managing cloud identity.

---

## Technologies Used
- Microsoft Entra ID (Azure Active Directory)
- Microsoft 365 Business Trial Tenant
- Microsoft Entra Admin Center (entra.microsoft.com)

---

## Lab Environment

| Resource | Details |
|---|---|
| Tenant | jjtechlab.onmicrosoft.com |
| Admin Account | Global Administrator |
| Test User | Jalen Ramsey (IT Technician) |

---

## What I Built

**User Creation** — Created a new user account in Entra ID for an IT Technician, configured properties including job title, department, and usage location, simulating an employee onboarding request processed through the identity management portal.

**Role Assignment** — Assigned the Helpdesk Administrator role to a user in Entra ID to simulate role-based access control, granting the user permission to reset passwords and manage service requests without providing full administrative privileges.

**Security Group Management** — Created an IT Technicians security group in Entra ID and added a user as a member, simulating role-based access control by grouping users by job function to manage permissions and resource assignments at the group level.

**Conditional Access** — Navigated to Conditional Access in Entra ID and reviewed the policy structure. Documented how Conditional Access uses an if/then model to enforce security controls such as requiring MFA based on conditions like user location, device compliance, or group membership.

**App Registration** — Registered an application in Entra ID to simulate how organizations integrate internal or third-party apps with Microsoft identity services, enabling single sign-on and centralized authentication management through the tenant.

**Sign-In Log Review** — Reviewed sign-in logs in Entra ID to monitor authentication activity across the tenant, demonstrating the ability to audit user access, investigate failed sign-in attempts, and identify suspicious authentication patterns.

---

## Table of Contents

| # | Section | Description |
|---|---|---|
| 01 | [User Creation](01-User-Creation/README.md) | Created a new Entra ID user with job title, department, and usage location |
| 02 | [Role Assignment](02-Role-Assignment/README.md) | Assigned Helpdesk Administrator role to simulate role-based access control |
| 03 | [Security Group Management](03-Security-Group-Management/README.md) | Created IT Technicians security group and added a member |
| 04 | [Conditional Access](04-Conditional-Access/README.md) | Reviewed Conditional Access policy structure and if/then model |
| 05 | [App Registration](05-App-Registration/README.md) | Registered an application in Entra ID for SSO and centralized authentication |
| 06 | [Sign-In Log Review](06-Sign-In-Log-Reviews/README.md) | Audited sign-in logs to monitor authentication activity across the tenant |

---

## Key Takeaways
- Created and configured user accounts in Entra ID simulating real employee onboarding workflows
- Practiced role-based access control by assigning the Helpdesk Administrator role without granting full admin privileges
- Created security groups to manage permissions at the group level rather than individually
- Understood how Conditional Access policies enforce security controls based on user and device conditions
- Registered an application in Entra ID to simulate enterprise SSO integration
- Audited sign-in logs to monitor authentication activity and identify suspicious patterns
