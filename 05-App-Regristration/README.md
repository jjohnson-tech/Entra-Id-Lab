## 05 - App Registration

App registration in Microsoft Entra ID allows organizations to integrate internal or third-party applications with Microsoft identity services. Once an app is registered, it can use Entra ID for authentication — enabling single sign-on (SSO), centralized access control, and secure API access through the tenant. In this section a new application was registered in Entra ID to simulate how IT and IAM teams onboard applications into the Microsoft identity platform.

---

## Step 1: Navigate to App Registrations

Logged into the Microsoft Entra admin center at **entra.microsoft.com**, expanded **Entra ID** in the left navigation panel, and selected **App registrations** to access the application management page.

<img width="1877" height="792" alt="app registration lading page" src="https://github.com/user-attachments/assets/e46c7177-c061-4dff-a7e8-2228025dadce" />


---

## Step 2: Create a New App Registration

Clicked **+ New registration** to begin registering a new application in the tenant.

<img width="1602" height="847" alt="app registration create" src="https://github.com/user-attachments/assets/15e5a82d-4bf9-47a0-a136-25bc4a8e05de" />


---

## Step 3: Configure the Application Details

Filled in the application registration details:

- **Name:** JJ Tech Lab Portal
- **Supported account types:** Accounts in this organizational directory only (Single tenant) — jjtechlab only

Single tenant means only users within the jjtechlab.onmicrosoft.com tenant can authenticate with this application. This is the appropriate setting for internal applications used exclusively within the organization.

The three account type options are:
- **Single tenant** — only users in this organization's directory
- **Multi-tenant** — users in any Microsoft Entra directory
- **Multi-tenant + personal Microsoft accounts** — broadest access including personal accounts

No redirect URI was configured for this registration since the app is a lab simulation and does not have an actual authentication endpoint.

<img width="1555" height="806" alt="jjtech registering app page" src="https://github.com/user-attachments/assets/79067bdf-3368-4d3e-87d2-31c6f3dd417a" />


---

## Step 4: Register the Application

Clicked **Register** to create the app registration in Entra ID. After registration, Entra ID automatically generated:

- **Application (client) ID** — a unique identifier for the application used in authentication requests
- **Directory (tenant) ID** — identifies the Entra ID tenant the application belongs to
- **Object ID** — the internal identifier for the app registration object in the directory

These IDs are used by developers and administrators when configuring the application to authenticate against Entra ID.

<img width="1541" height="757" alt="jjtech application registration confirmation" src="https://github.com/user-attachments/assets/46b4f53d-c35f-42f9-996c-9fa3a62d96b9" />


---

## Step 5: Confirm the App Appears in App Registrations

Navigated back to **App registrations** and confirmed the **JJ Tech Lab Portal** appeared in the list of registered applications with the correct application ID and tenant association.

<img width="1547" height="767" alt="app confirmatin listed" src="https://github.com/user-attachments/assets/d20c7f3d-a597-4624-b7f9-2b4267152349" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to App Registrations | Opened App registrations under Entra ID |
| Create New Registration | Clicked + New registration |
| Configure Details | Set app name and single tenant account type |
| Register Application | Clicked Register to provision the app in Entra ID |
| Note Generated IDs | Documented Application ID, Directory ID, and Object ID |
| Confirm Registration | Verified app appeared in the App registrations list |

App registration is a fundamental IAM and cloud administration task. Registering applications in Entra ID enables organizations to centrally manage which apps can authenticate users through their tenant, enforce access policies, and maintain visibility over third-party and internal application integrations — all critical responsibilities for IAM Analysts and Systems Administrators working in Microsoft 365 environments.
