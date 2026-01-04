## 📋 Enrollment Status Page (ESP)

The Enrollment Status Page (ESP) is configured to control the Windows Autopilot deployment experience and ensure devices are fully provisioned before first use.

### 🔧 Key Behaviors
- Display installation progress during Out-of-Box Experience (OOBE)
- Block user access until required apps and profiles are installed
- Track provisioning status of devices and applications
- Show error information if installation exceeds defined time limits

Blocking applications include core productivity and management components such as **Company Portal** and **Microsoft 365 Apps**.

![ESP Configuration - Settings](screenshots/autopilot-esp-settings.png)
![ESP Configuration - Basics](screenshots/esp-settings-first-page.png)

---

## Why These ESP Settings Matter

The ESP configuration is designed to balance deployment reliability, security, and user experience during Windows Autopilot provisioning.

### Blocking Until Apps and Profiles Are Installed
Ensures devices are compliant and operational before first use, reducing post-deployment support incidents.

###  Visibility of Deployment Progress
Provides transparency during OOBE, helping users understand setup status and reducing support calls.

### Error Handling and Recovery
Enables timeout messaging and recovery options (e.g., reset or retry), minimizing IT intervention.

### Scoped to Autopilot-Provisioned Devices
Applies only to devices provisioned via OOBE, avoiding impact on manually enrolled or legacy devices.

### Controlled Application Blocking
Limits blocking to essential apps (e.g., Company Portal), improving reliability while ensuring readiness.

---

##  Skills Demonstrated in This Repository

This repository showcases practical experience aligned with the responsibilities of a Microsoft Intune / Endpoint Engineer.

###  Device Provisioning & Lifecycle Management
- Designed and implemented Windows Autopilot user-driven deployments
- Configured Azure AD (Entra ID) join for cloud-native onboarding
- Implemented pre-provisioning to reduce end-user setup time

###  Intune Configuration & Policy Management
- Created configuration profiles for security and device control
- Designed ESP behavior to enforce deployment quality
- Managed application deployment and dependencies during OOBE

###  Identity & Access Integration
- Integrated Microsoft Entra ID with Windows Autopilot
- Applied dynamic device groups for automated policy assignment

###  Operational Excellence & Supportability
- Reduced first-day support incidents through proactive design
- Enabled visibility, error handling, and recovery mechanisms
- Documented architecture and configuration for handover

###  Security & Best Practices
- Enforced standard user access during provisioning
- Ensured compliance before granting access
- Followed Microsoft-recommended Autopilot and Intune design patterns

---

##  Use Cases

This deployment model is ideal for:
- New employee device provisioning
- Device refresh and replacement
- Remote-first or hybrid work environments
- Zero-touch delivery scenarios
