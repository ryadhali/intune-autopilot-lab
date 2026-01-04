Windows Autopilot & Intune Deployment Lab
A complete end‑to‑end modern device provisioning project

This repository documents a full Windows Autopilot deployment lab built using Microsoft Intune (Endpoint Manager). It demonstrates real‑world skills in device provisioning, security configuration, identity integration, and operational readiness for enterprise environments.

The project includes device registration, deployment profiles, Enrollment Status Page (ESP) configuration, dynamic device groups, configuration profiles, application deployment, and compliance controls — all aligned with Microsoft best practices.

Table of Contents
Overview

01 Device Registration

02 Deployment Profile

03 Enrollment Status Page (ESP)

04 Dynamic Device Groups

05 Configuration Profiles

06 Apps & Compliance

Skills Demonstrated

Use Cases

Overview
This lab simulates a full modern device provisioning workflow using Windows Autopilot and Microsoft Intune. It is designed to reflect the responsibilities of an Intune / Endpoint Engineer, including:

Cloud‑native device onboarding

Zero‑touch provisioning

Security and compliance enforcement

Application deployment

Identity and access integration

Operational readiness and monitoring

Each section includes screenshots, configuration examples, and explanations of why specific settings were chosen.

01 Device Registration
Devices are registered into Windows Autopilot using hardware hashes.
This enables:

Zero‑touch provisioning

Automatic profile assignment

Consistent device lifecycle management

Folder includes:

Hardware hash import

Device registration validation

Autopilot device list screenshots

02 Deployment Profile
The Autopilot deployment profile defines the Out‑of‑Box Experience (OOBE) for end users.

Key settings include:

User‑driven mode

Azure AD Join

Language and keyboard configuration

Privacy settings (hidden)

Standard user account enforcement

Device naming template

This ensures a streamlined, secure, and predictable setup experience.

03 Enrollment Status Page (ESP)
The ESP ensures devices are fully configured before the user reaches the desktop.

Key behaviours:

Show installation progress

Block access until required apps/profiles install

Track provisioning status

Display error information and allow recovery

Blocking apps include essential components such as Company Portal and Microsoft 365 Apps.

Screenshots included:

ESP basics

ESP settings

Blocking apps configuration

04 Dynamic Device Groups
Dynamic device groups automate assignment of Autopilot profiles, configuration policies, and applications.

Example membership rule:

(device.devicePhysicalIds -any (_ -eq "[OrderID]:RALI_Testing"))
and
(device.devicePhysicalIds -any (_ -contains "[ZTDId]"))

This ensures only Autopilot‑registered devices with a specific OrderID tag are included.

05 Configuration Profiles
Configuration profiles standardise device configuration and enforce security across all Autopilot‑provisioned devices.

User Experience & OS Configuration
Examples:

Chrome homepage

Taskbar layout

Time zone

SAP pop‑up permissions

Standard user reset options

Security Baseline & Device Hardening
Examples:

LAPS

Attack Surface Reduction (ASR)

Exploit protection

Windows security policies

Microsoft Defender & Identity Protection
Examples:

Defender onboarding

SAM‑R configuration

Antivirus and real‑time protection

Firewall & Network Configuration
Examples:

Windows Firewall rules

Miracast exceptions

Enterprise app rules

Update, Health & Compliance
Examples:

Update rings

Health monitoring

Restart behaviour

Custom & ADMX‑Based Policies
Examples:

ADMX imports

Root CA certificates

Registry‑based custom settings

06 Apps & Compliance
This section includes:

Application deployment (Win32, Store, LOB)

Required vs available apps

Compliance policies

Conditional access alignment

Company Portal configuration

Applications are deployed during ESP or immediately after enrollment to ensure readiness at first sign‑in.

Skills Demonstrated
This project demonstrates hands‑on experience in:

Device Provisioning & Lifecycle
Autopilot user‑driven deployments

Azure AD Join

Pre‑provisioning (White Glove)

Intune Configuration & Policy Management
Security baselines

ASR rules

Update rings

Firewall and Defender configuration

Identity & Access
Microsoft Entra ID integration

Dynamic device groups

Role‑based access alignment

Operational Excellence
Reducing first‑day support incidents

Error handling and recovery

Documentation and handover readiness

Security Best Practices
Standard user enforcement

Compliance before access

Hardening via ASR, LAPS, Defender

Use Cases
This deployment model is ideal for:

New employee onboarding

Device refresh cycles

Remote and hybrid workforces

Zero‑touch device delivery

Scalable enterprise provisioning
