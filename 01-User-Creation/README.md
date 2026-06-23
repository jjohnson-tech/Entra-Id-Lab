## 01 - User Creation

Creating user accounts in Microsoft Entra ID is one of the most fundamental identity management tasks in a Microsoft 365 environment. In this section a new user account was created for an IT Technician, simulating a real employee onboarding request processed through the Entra ID admin center. User properties including job title, department, and usage location were configured to reflect how accounts are set up in enterprise environments.

---

## Step 1: Navigate to Microsoft Entra ID

Logged into the Microsoft Entra admin center at **entra.microsoft.com** using the Global Administrator account. The Entra admin center is the central hub for managing identities, access, and security across the Microsoft 365 tenant.

<img width="1907" height="866" alt="entra admin center landing page" src="https://github.com/user-attachments/assets/6c6f8225-ecdf-49cb-89ed-c8976748efa8" />


---

## Step 2: Navigate to Users

In the left navigation panel, clicked **Users → All Users** to open the user management page. This page displays all user accounts in the tenant and provides options to create, manage, and delete accounts.

<img width="1552" height="472" alt="users listed" src="https://github.com/user-attachments/assets/b9eb9da2-7fab-49b5-b236-92f0f0207143" />


---

## Step 3: Create a New User

Clicked **+ New user → Create new user** to begin creating a new user account. The create new user option provisions a cloud-only account directly in Entra ID — as opposed to inviting an external guest user.

<img width="1547" height="793" alt="creating user page jr" src="https://github.com/user-attachments/assets/43db5eb3-0ee5-4f54-a4a4-6c92c1f65a25" />


---

## Step 4: Configure User Identity

Filled in the user identity details:

- **Display name:** Jalen Ramsey
- **User principal name:** jramsey@jjtechlab.onmicrosoft.com
- **Mail nickname:** jramsey (auto-generated)
- **Password:** Auto-generated temporary password with user required to change at first sign-in

The user principal name (UPN) is the user's login username — it must be unique across the tenant and follows the format username@domain.

<img width="1547" height="785" alt="jram user details" src="https://github.com/user-attachments/assets/72f9fcf6-2f88-4268-92f0-2c22e6802a0a" />


---

## Step 5: Configure User Properties

Navigated to the **Properties** tab and filled in additional user details to simulate a real onboarding request:

- **Job title:** IT Technician
- **Department:** Information Technology
- **Usage location:** United States

Setting the usage location is required before a Microsoft 365 license can be assigned to the user — it determines which services and compliance regulations apply based on the user's region.

<img width="1671" height="810" alt="jram additional info" src="https://github.com/user-attachments/assets/1584ec32-94f4-4a5f-aff3-14987a0da114" />

---

## Step 6: Review and Create the User

Reviewed all the configured settings on the **Review + create** tab to verify everything was correct before creating the account. Clicked **Create** to provision the user account in Entra ID.

<img width="1887" height="817" alt="jram review and create" src="https://github.com/user-attachments/assets/fc6bc357-3876-4e25-bbdb-7e8cf4cafa1e" />


---

## Step 7: Confirm the User Appears in All Users

After creation, navigated back to **Users → All Users** and confirmed the **Jalen Ramsey** account appeared in the user list with the correct UPN and account status showing as active.

<img width="1538" height="742" alt="jr showing in user list" src="https://github.com/user-attachments/assets/cde6bd3e-c8a4-4791-93c1-3e2d42d5328e" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Entra ID | Opened the Entra admin center at entra.microsoft.com |
| Navigate to Users | Opened All Users from the left navigation panel |
| Create New User | Selected New user → Create new user |
| Configure Identity | Set display name, UPN, and temporary password |
| Configure Properties | Set job title, department, and usage location |
| Review and Create | Verified settings and created the account |
| Confirm User | Verified Jalen Ramsey appeared in the All Users list |

User creation in Entra ID is one of the most common IAM tasks performed by helpdesk and sysadmin teams. Configuring the correct properties during account creation — especially usage location — ensures the account is ready for license assignment and acc
