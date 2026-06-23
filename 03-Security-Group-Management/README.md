## 03 - Security Group Management

Security groups in Microsoft Entra ID are used to manage access to resources by grouping users together based on job function, department, or role. Instead of assigning permissions to individual users, permissions are assigned to the group — making it easy to manage access at scale. In this section an IT Technicians security group was created in Entra ID and Jalen Ramsey was added as a member, simulating how organizations use group-based access control in enterprise environments.

---

## Step 1: Navigate to Groups

Logged into the Microsoft Entra admin center at **entra.microsoft.com** and navigated to **Groups → All Groups** to access the group management page.

<img width="1857" height="725" alt="all groups showing" src="https://github.com/user-attachments/assets/097df9c7-d1b4-4e5e-9090-58a936c3b9ba" />


---

## Step 2: Create a New Group

Clicked **+ New group** to begin creating a new security group. Configured the group type settings:

- **Group type:** Security
- **Group name:** IT Technicians
- **Group description:** Security group for IT Technician staff — used for managing permissions and resource access by job function
- **Membership type:** Assigned — members are manually added by an administrator

Security groups are used specifically for access control and permission management. The Assigned membership type means administrators manually control who is in the group, as opposed to Dynamic membership which automatically adds users based on user attributes.

<img width="1902" height="817" alt="new group details" src="https://github.com/user-attachments/assets/596bb093-341c-42ee-a86d-7f2c9305124a" />


---

## Step 3: Add a Member During Group Creation

Before clicking Create, clicked **No members selected** under the Members section to add a member to the group during creation. Searched for and selected **Jalen Ramsey** to add as the first member of the IT Technicians group.

<img width="1836" height="732" alt="add jram to sec group" src="https://github.com/user-attachments/assets/433c9dd7-56ce-449d-811e-6d77c1339f75" />


---

## Step 4: Create the Group

Clicked **Create** to provision the IT Technicians security group with Jalen Ramsey as a member.

<img width="1552" height="760" alt="new group creation page" src="https://github.com/user-attachments/assets/70d313a0-0126-4ad6-81eb-90bb82ef0e45" />


---

## Step 5: Confirm the Group Appears in All Groups

Navigated back to **Groups → All Groups** and confirmed the **IT Technicians** security group appeared in the list with the correct group type and membership count.

<img width="1822" height="772" alt="it tech group showing" src="https://github.com/user-attachments/assets/ccd59e0d-80d1-4112-9505-9cee64e33182" />


---

## Step 6: Verify Member in the Group

Clicked into the **IT Technicians** group and navigated to the **Members** tab to confirm Jalen Ramsey was listed as an active member of the group.

<img width="1490" height="797" alt="jram member added " src="https://github.com/user-attachments/assets/55823479-135b-40df-8d77-0b72e46bb0cf" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Groups | Opened All Groups in the Entra admin center |
| Create New Group | Clicked + New group and configured Security type |
| Configure Details | Set group name, description, and Assigned membership type |
| Add Member | Added Jalen Ramsey as a member during group creation |
| Create Group | Clicked Create to provision the IT Technicians group |
| Confirm Group | Verified group appeared in All Groups list |
| Verify Member | Confirmed Jalen Ramsey was listed on the Members tab |

Security group management is a fundamental IAM skill. Managing access at the group level rather than the individual user level is the standard approach in enterprise environments — when a new IT Technician is hired, they are simply added to the IT Technicians group and immediately inherit all the correct permissions without any additional configuration.
