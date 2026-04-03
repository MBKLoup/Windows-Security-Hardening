# Windows Security Hardening Lab

## Overview

This project focused on hardening a Windows 10 system using industry-standard security configurations. I worked through a baseline system, identified default security weaknesses, and implemented controls to strengthen authentication, logging, and system services.

The goal was to simulate what a system administrator or security analyst would do when preparing a workstation for enterprise use: enforce strong authentication policies, enable auditing for visibility, and reduce the attack surface by reviewing system services.

---

## Environment

- Windows 10 Virtual Machine  
- VirtualBox  
- Local Security Policy (secpol.msc)  
- Services Manager (services.msc)  
- Event Viewer  

---

## Phase 1 — Baseline Review

Before making any changes, I reviewed the system’s default configuration to understand its security posture.

### What I checked

  - Password policy settings (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/DefulatPasswordSettings.png)
  - Account lockout policy  (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/DefaultAccountLockoutPolicy.png)
  - Audit policy configuration  (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/DefaultAuditPolicies.png)
  
  - List of running services  (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/DefaultRunningServices1.png) 1/2
  - (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/DefaultRunningServices2.png) 2/2
  

---

## Phase 2 — Authentication Hardening

I configured password and account lockout policies to enforce stronger authentication.

### Changes implemented
  ## Password (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/HardenedPasswordSettings.png)
-   Enabled password complexity requirements  
-   Increased minimum password length

  ## Account Settings (https://github.com/MBKLoup/Windows-Security-Hardening/blob/main/Screenshots/HardenedAccountSettings.png)
-   Configured account lockout threshold  
-   Set lockout duration and reset timers  


---

## Phase 3 — Audit Logging Configuration

I enabled auditing to ensure that important system events are logged and can be reviewed.

### Audit categories enabled

- Logon and logoff events  
- Account management  
- Policy changes  
- Privilege use  

---

## Phase 4 — Service Hardening

I reviewed the list of running services to identify unnecessary or potentially risky services.

### What I did

- Analyzed running services in services.msc  
- Evaluated whether each service was required for a workstation  
- Disabled non-essential services where appropriate  

---

## Phase 5 — Local Security Options

I configured additional local security settings to improve system protection and user awareness.

### Changes implemented

- Enabled an interactive logon message  
- Reviewed administrator account settings  
- Adjusted security-related local policies  

---

## Phase 6 — Testing & Validation

After applying all configurations, I verified that the changes were working as expected.

### Tests performed

- Attempted multiple failed logins to trigger account lockout  
- Performed successful login to confirm access  
- Generated audit events through account and policy changes  
- Reviewed logs in Event Viewer  

---

## Challenges & Observations

- Lack of Group Policy Editor on Windows 10 Home  
- Large number of system services  
- Audit log volume considerations  

---

## Practical Applications

- System hardening for enterprise workstations  
- Audit logging for incident detection  
- Account policies to prevent unauthorized access  
- Service management to reduce attack surface  

---

## What I Learned

- Configuring Windows security policies  
- Importance of authentication controls  
- How audit logs support monitoring  
- Evaluating system services for security  
- Validating configurations  

---


---

## Skills Demonstrated

- Windows System Hardening  
- Security Configuration  
- Log Analysis  
- Risk Reduction  
- Troubleshooting  

---

## Author

Kalala | Cybersecurity & IT  
