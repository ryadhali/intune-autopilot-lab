Applications
Applications are deployed automatically during Windows Autopilot provisioning to ensure devices are ready for use at first sign-in.

Apps are targeted using dynamic device groups and assigned as Required where necessary to enforce consistency and readiness.

Application Types
Microsoft 365 Apps

Microsoft Company Portal

Win32 line-of-business applications

Security and management agents

Critical applications are installed during the Enrollment Status Page (ESP) phase to prevent users from accessing partially configured devices.

Application Deployment Examples
Required application overview (Win32 / Microsoft apps):  
[Looks like the result wasn't safe to show. Let's switch things up and try something else!]

Application assignment targeting dynamic device groups:  
[Looks like the result wasn't safe to show. Let's switch things up and try something else!]

Additional screenshots (e.g., VPN client, Company Portal, productivity tools) are omitted to avoid exposing organisation-specific implementation details.

Compliance Policies
Compliance policies evaluate device health and enforce minimum security requirements for managed Windows devices.

Devices that do not meet compliance standards can be restricted from accessing organisational resources.

Example Compliance Controls
BitLocker encryption enabled

Secure Boot enabled

Minimum supported Windows version

Password and device security requirements

Policies are assigned using dynamic device groups to ensure consistent evaluation across all Autopilot-provisioned devices.

Compliance Policy Example
Compliance policies are designed to integrate with Conditional Access, controlling access to cloud resources based on device health status.