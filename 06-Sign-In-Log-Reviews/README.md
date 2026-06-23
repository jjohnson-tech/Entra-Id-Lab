## 06 - Sign-In Log Review

Sign-in logs in Microsoft Entra ID provide a detailed record of every authentication attempt across the tenant — including successful logins, failed attempts, the application accessed, the IP address, location, and any error codes associated with the sign-in. Reviewing sign-in logs is a core security and auditing task performed by IAM analysts, sysadmins, and helpdesk teams to monitor user access, investigate suspicious activity, and troubleshoot authentication issues.

---

## Step 1: Navigate to Sign-In Events

Logged into the Microsoft Entra admin center at **entra.microsoft.com**, expanded **Entra ID** in the left navigation panel, and navigated to **Monitoring & health → Sign-in events** to access the authentication audit logs for the tenant.

<img width="1917" height="816" alt="signinlog landing page" src="https://github.com/user-attachments/assets/53b25564-f286-456e-93c8-752a62946979" />


---

## Step 2: Review the Sign-In Events Overview

The sign-in events page displays authentication activity organized across four tabs:

- **User sign-ins (interactive)** — logins where the user actively entered credentials
- **User sign-ins (non-interactive)** — background token refreshes and app authentications that don't require user input
- **Service principal sign-ins** — authentications from apps and services using their own identity
- **Managed identity sign-ins** — authentications from Azure resources using managed identities

The **User sign-ins (interactive)** tab was reviewed as it shows the most relevant activity for helpdesk and IAM auditing. Each entry displays:

- **Date** — timestamp of the authentication event in UTC
- **Request ID** — unique identifier for the sign-in request
- **User principal name** — the account that authenticated
- **Application** — the app or service accessed
- **Status** — Success or Failure
- **IP address** — the source IP of the sign-in attempt
- **Resource** — the specific Microsoft resource accessed

<img width="1917" height="816" alt="signinlog landing page" src="https://github.com/user-attachments/assets/fbf6c886-272c-4112-b860-079491dad4db" />


---

## Step 3: Use Add Filter to Narrow Results

Clicked **Add filter** to filter the sign-in events by specific criteria. Available filters include:

- **User** — filter by a specific user account
- **Application** — filter by a specific app such as Azure Portal or Microsoft Teams
- **Status** — filter by Success or Failure
- **Date range** — adjust the time window (default is Last 24 hours)
- **IP address** — filter by a specific source IP

Filtering by user is the standard approach when investigating a specific account — such as responding to a helpdesk ticket about a login issue or auditing access after an account was flagged.

<img width="1607" height="817" alt="filter sign in events by user" src="https://github.com/user-attachments/assets/c9572f50-787f-48ed-91f3-179b6500ba43" />



---

## Step 4: Click Into a Sign-In Event for Details

Clicked on an individual sign-in event to open the detailed view. The detail panel provides additional information including:

- **Authentication method** — how the user authenticated
- **Conditional Access policies** — which policies were evaluated
- **Device information** — device name and operating system
- **Location** — geographic location of the sign-in
- **Error code** — for failed sign-ins, the reason for failure

Common sign-in error codes include:

| Error Code | Meaning |
|---|---|
| 50126 | Invalid username or password |
| 50057 | Account is disabled |
| 50076 | MFA required but not completed |
| 53003 | Access blocked by Conditional Access policy |
| 50055 | Password expired |

<img width="1835" height="807" alt="sign in details addtional info" src="https://github.com/user-attachments/assets/bfe15b8a-9dc8-40aa-b4d8-e0618c3a990f" />


---

## Step 5: Review the Export and Download Options

Noted the **Download** and **Export data settings** options at the top of the Sign-in events page. In enterprise environments these options are used to:

- Export sign-in logs to a SIEM tool like Microsoft Sentinel for long-term retention and alerting
- Download logs as CSV or JSON for offline analysis
- Set up diagnostic settings to stream logs to a Log Analytics workspace

<img width="1907" height="417" alt="options visible" src="https://github.com/user-attachments/assets/6995a823-e02c-4ddf-beaf-2bc1a90c8d4f" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Sign-In Events | Opened Monitoring & health → Sign-in events in Entra ID |
| Review Tabs | Reviewed the four sign-in tabs — interactive, non-interactive, service principal, managed identity |
| Review Log Columns | Noted date, user, application, status, IP address, and resource columns |
| Add Filter | Used Add filter to narrow events by user, application, or status |
| Review Event Detail | Clicked into an event to see authentication method, device, and error codes |
| Review Export Options | Noted Download and Export data settings for SIEM integration |

Sign-in event review is one of the most practical security and troubleshooting skills in Microsoft Entra ID. Whether responding to a user login issue, investigating a suspicious sign-in, or auditing access after a security incident — the sign-in events page is the first place to look. Knowing how to navigate, filter, and interpret sign-in data is an essential skill for helpdesk, IAM, and security roles in any Microsoft 365 environment.
