## Autopilot Deployment Profile

**Path:**  
Devices → Windows → Windows enrollment → Deployment Profiles → AP-UserDriven-Standard

### Deployment Type
This deployment uses a **User-driven Windows Autopilot profile** with
**Microsoft Entra ID (Azure AD) Join**.

Devices are joined directly to Entra ID during the Out-of-Box Experience (OOBE),
providing a cloud-native, zero-touch deployment model suitable for modern
enterprise environments.

### OOBE Configuration
Key Out-of-Box Experience settings include:
- User-driven deployment
- Microsoft Entra ID (Azure AD) Join
- Standard user account
- Pre-provisioning enabled to reduce end-user setup time
- Automated device naming using a template

![Autopilot Deployment Profile Overview](screenshots/deployment-profile-overview.png)

Pre-provisioning ensures that required applications and policies are applied
before the device is handed over to the end user.

deployment-profile-overview
