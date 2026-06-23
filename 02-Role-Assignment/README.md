## 02 - Role Assignment

Role assignment in Microsoft Entra ID controls what administrative actions a user can perform within the tenant. Instead of giving every IT staff member full Global Administrator access, roles are assigned based on the principle of least privilege — granting only the permissions needed to perform specific job functions. In this section the Helpdesk Administrator role was assigned to Jalen Ramsey, simulating how IT teams delegate limited admin access to helpdesk staff.

---

## Step 1: Navigate to the User Account

Logged into the Microsoft Entra admin center at **entra.microsoft.com** and navigated to **Users → All Users**. Located and clicked on the **Jalen Ramsey** account to open the user details page.

<img width="1538" height="742" alt="jr showing in user list" src="https://github.com/user-attachments/assets/bd1542a4-4e90-4e8f-b18b-7a65dee4fa92" />


---

## Step 2: Open Assigned Roles

Inside the Jalen Ramsey user details page, clicked **Assigned roles** in the left navigation panel to view any existing role assignments and access the option to add a new role.

<img width="1607" height="797" alt="jram role assignment" src="https://github.com/user-attachments/assets/f1fa2933-97d7-4a2b-ad65-3a2ee2a38027" />


---

## Step 3: Add Assignment

Clicked **+ Add assignments** to open the role selection panel and search for the role to assign.

<img width="1597" height="822" alt="jram add assignment" src="https://github.com/user-attachments/assets/4fa3ec7b-9fe4-46c1-a559-aaf14cd13eb2" />


---

## Step 4: Search for and Select the Helpdesk Administrator Role

In the role selection panel, searched for **Helpdesk Administrator** and selected it from the results. The Helpdesk Administrator role grants the user permission to:

- Reset passwords for non-administrator users
- Manage service requests
- Monitor service health

This role does not grant access to sensitive admin functions like managing other administrators or configuring security policies — making it appropriate for helpdesk staff who need to handle common user support tasks without full admin access.

<img width="1607" height="815" alt="jram helpdesk role selected" src="https://github.com/user-attachments/assets/09adcda0-fdad-47fc-b86b-2134cd36bb10" />


---

## Step 5: Confirm the Role Assignment

Clicked **Add** to apply the role assignment. Confirmed the **Helpdesk Administrator** role appeared in the Assigned roles list for Jalen Ramsey with the assignment type showing as Active.

<img width="1550" height="787" alt="jram assigned to helpdesk admin role" src="https://github.com/user-attachments/assets/93fbec7e-f86e-4941-9578-9d85dd97961c" />

---

## Summary

| Task | Action |
|---|---|
| Navigate to User | Opened Jalen Ramsey's account in Entra admin center |
| Open Assigned Roles | Clicked Assigned roles in the user details panel |
| Add Assignment | Clicked + Add assignments to open role selection |
| Select Role | Searched for and selected Helpdesk Administrator |
| Confirm Assignment | Verified role appeared as Active in Assigned roles list |

Role assignment is a core IAM task in Entra ID. Assigning the Helpdesk Administrator role rather than Global Administrator follows the principle of least privilege — a fundamental security practice that limits the damage a compromised or misused account can cause by ensuring users only have the access they actually need to do their job.
