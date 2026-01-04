**Path:**  
Intune admin center → Devices → Windows → Configuration profiles

## Configuration Profiles

Configuration profiles are used to standardise device configuration,
enforce security controls, and provide a consistent user experience
across all Windows devices provisioned via Windows Autopilot.

Profiles are scoped using dynamic device groups and are applied during
Autopilot provisioning or immediately after device enrollment.

---

### 1. User Experience & OS Configuration
These profiles ensure a consistent and controlled end-user environment.

Examples include:
- Google Chrome homepage configuration
- Removal of Microsoft Store from the taskbar
- Personalisation settings
- Time zone configuration
- Enable standard user PC reset
- SAP application – allow pop-up permissions

These settings reduce user friction while maintaining organisational standards.

---

### 2. Security Baseline & Device Hardening
Security-focused profiles enforce core endpoint protection and hardening controls.

Examples include:
- Local Administrator Password Solution (LAPS)
- Attack Surface Reduction (ASR) rules
- Windows security policy settings
- Exploit protection configuration

These controls reduce the device attack surface and align with Microsoft
security best practices.

![Security Configuration Profile](screenshots/config-security-settings.png)

---

### 3. Microsoft Defender & Identity Protection
These profiles integrate endpoints with Microsoft Defender and identity
protection services.

Examples include:
- Microsoft Defender onboarding
- Microsoft Defender for Identity – SAM-R configuration
- Endpoint exploit protection
- Antivirus and real-time protection settings

This ensures devices are monitored and protected from first sign-in.

![Defender Profile Overview](screenshots/config-defender-overview.png)

---

### 4. Firewall & Network Configuration
Firewall profiles manage network access and application communication.

Examples include:
- Windows Firewall rules
- Firewall exceptions for Miracast
- Custom firewall rules for enterprise applications

These profiles allow required services while maintaining a secure network posture.

---

### 5. Update, Health & Compliance
These profiles manage device lifecycle, update behaviour, and operational health.

Examples include:
- Windows Update rings
- Device health monitoring configuration
- Restart and update behaviour controls

This ensures devices remain secure, up to date, and compliant over time.

![Windows Update Ring](screenshots/config-update-ring.png)

---

### 6. Custom & ADMX-Based Configuration
Custom and ADMX-based policies are used where built-in Intune settings are insufficient.

Examples include:
- Imported ADMX templates
- Root CA certificate deployment
- Custom registry-backed configurations

This demonstrates the ability to extend Intune beyond default configuration options.

![ADMX Profile Example](screenshots/config-admx-example.png)

---

Additional configuration profiles exist for certificate trust, enterprise
application support, and advanced firewall configuration. These are
documented at a high level only to avoid exposing sensitive or
organisation-specific settings.
