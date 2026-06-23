## 04 - Conditional Access

Conditional Access is Microsoft Entra ID's policy engine for enforcing security controls based on specific conditions. It uses an if/then model — if a user meets certain conditions such as signing in from an unfamiliar location, using an unmanaged device, or belonging to a specific group, then a control is enforced such as requiring MFA, blocking access, or limiting what the user can do.

In this section the Conditional Access area was navigated to and reviewed in the Entra admin center. Full policy creation and management requires an **Entra ID Premium P1** license which is not included in the Microsoft 365 Business trial tenant used in this lab. The policy structure and capabilities were reviewed and documented to demonstrate understanding of how Conditional Access works in enterprise environments.

---

## Step 1: Navigate to Conditional Access

Logged into the Microsoft Entra admin center at **entra.microsoft.com**, expanded **Entra ID** in the left navigation panel, scrolled down, and selected **Conditional Access**.

<img width="1887" height="842" alt="cond access policy" src="https://github.com/user-attachments/assets/172cfc82-25d1-48ce-b6cc-b935d983e4e1" />


---

## Step 2: Review the Conditional Access Overview Page

The Conditional Access overview page was displayed. Due to the Microsoft 365 Business trial license, full policy creation was not available. The overview page shows the policy management interface and confirms that Entra ID Premium P1 licensing is required to create and enforce Conditional Access policies.

<img width="1882" height="815" alt="condtional overview" src="https://github.com/user-attachments/assets/f256c958-336f-4bca-85d7-723249cbefa6" />


---

## Step 3: Understand the Conditional Access Policy Model

Although full policy creation was not available in this trial tenant, Conditional Access was studied and documented based on Microsoft's official documentation. Every Conditional Access policy is built around three components:

**Assignments — Who and What the policy applies to:**
- **Users** — specific users, groups, or roles the policy targets
- **Target resources** — specific apps or all cloud apps the policy applies to
- **Conditions** — additional filters such as sign-in risk level, device platform, location, or client app type

**Access controls — What happens when conditions are met:**
- **Grant** — allow access with additional requirements such as requiring MFA, requiring a compliant device, or requiring a specific authentication strength
- **Block** — deny access entirely when conditions are met
- **Session** — limit what the user can do within an app even after access is granted

**Common enterprise Conditional Access policies include:**
- Require MFA for all users signing in from outside the corporate network
- Block access from high-risk sign-in locations
- Require a compliant device for access to sensitive applications
- Block legacy authentication protocols that do not support MFA

---

## Summary

| Component | Description |
|---|---|
| Users | Who the policy applies to — specific users, groups, or roles |
| Target Resources | Which apps the policy covers — specific apps or all cloud apps |
| Conditions | Additional filters — sign-in risk, device platform, location, client app |
| Grant | Allow access with requirements such as MFA or compliant device |
| Block | Deny access entirely when conditions are met |
| Session | Limit what the user can do within an app after access is granted |
| License Required | Entra ID Premium P1 required for full policy creation and enforcement |

Conditional Access is one of the most powerful security tools in Microsoft Entra ID. Understanding the if/then policy model is essential knowledge for anyone working in IAM, security administration, or helpdesk roles in a Microsoft 365 environment. Full implementation would be explored further with a Premium P1 license.
