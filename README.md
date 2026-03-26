**Windows Enterprise Identity & Access Control Hardening**

**Overview**

This project demonstrates the configuration and validation of core Windows Enterprise security controls on a standalone workstation. 

The lab focuses on identity and access management, auditing, and system service hardening using built-in Windows security tools.

**Objectives**

\- Establish a baseline security configuration

\- Configure password and account lockout policies

\- Enable and validate security auditing

\- Harden selected system services

\- Validate security controls through event logs

**Environment**

\- Host OS: Windows

\- Virtualization: VirtualBox

\- Guest OS: Windows 10 Enterprise Evaluation (64-bit)

\- Tools: Local Security Policy, Services MMC, Event Viewer, PowerShell

**Lab Steps**

1\. Baseline security configuration review

2\. Password and account lockout policy configuration

3\. Audit policy configuration

4\. System service hardening

5\. Security options hardening

6\. Validation and testing

**Key Security Controls Implemented**

\- Account lockout and password complexity enforcement

\- Logon, account management, and policy change auditing

\- Interactive logon warning banner

\- Disabled built-in Administrator account

\- Reduced attack surface through selective service hardening

**Validation**

Security controls were validated using controlled logon attempts and review of the Windows Security Event Log.

**Skills Demonstrated**

\- Windows security hardening

\- Identity and access control

\- Audit logging and event analysis

\- Security baseline documentation

\- Virtualized lab environments