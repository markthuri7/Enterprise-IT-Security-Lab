# Enterprise IT & Security Home Lab

## Overview
This project documents a Windows enterprise lab environment built to practice IT support and cybersecurity operations.

The lab simulates a corporate network with centralized authentication, endpoint management, and security monitoring.

## Technologies Used
- Windows Server 2022 (Domain Controller)
- Active Directory & DNS
- Windows 11 Pro Client
- VirtualBox
- Ubuntu Server - Wazuh SIEM
- Internal Network (LabNet)

## Lab Architecture
- DC01 – Domain Controller, DNS
- PC01 – Domain Client
- Domain: lab.local

## Key Skills Demonstrated
- Installed and configured Active Directory Domain Services
- Created and managed domain users
- Joined Windows clients to domain
- Configured DNS and static IPs
- Troubleshot connectivity and authentication issues
- Implemented Group Policy to enforce automatic screen lock and password protection
- Verified policy deployment using gpresult and gpupdate
- Created file shares and implemented NTFS and share permissions
- Deployed Group Policy drive mapping based on security groups
- Configured domain password and account lockout policies
- Performed account unlocks and password resets using GUI and CLI
- Installed and secured osTicket on Windows using XAMPP
- Created agent and user roles
- Managed ticket lifecycle from submission to resolution
- Documented incident response workflows
- Using Wazuh I detected and investigated failed logins (Event ID 4625), account lockouts (Event ID 4740) and privilege escalation (Event ID 4732)

## Screenshots

### Active Directory Users
![AD Users](screenshots/ad-users.png)

### Server Manager
![Server Manager](screenshots/server-manager.png)

### Domain Membership
![PC01 Domain](screenshots/pc01-domain.png)

### Domain Login
![Domain Login](screenshots/domain-login.png)

### Network Test
![Ping Test](screenshots/ping-test.png)

### Group Policy – Screen Lock Enforcement
![GPO Settings](screenshots/gpo-screenlock-settings.png)
![Locked Screen](screenshots/pc01-screen-locked.png)

### File Server and Drive Mapping
![Drive Mapping GPO](screenshots/gpo-drive-mapping.png)
![Shares](screenshots/company-shares-structure.png)
![Mapped Drive](screenshots/mapped-drive-it.png)

### Password Policy and Account Management
![Password Policy](screenshots/password-policy.png)
![Lockout Policy](screenshots/lockout-policy.png)
![Locked Account](screenshots/account-locked.png)
![Password Reset](screenshots/password-reset.png)

### Helpdesk Ticketing System (osTicket)
![Admin Dashboard](screenshots/ticket-admin-dashboard.png)
![Open Ticket](screenshots/ticket-open-admin.png)
![Resolved Ticket](screenshots/ticket-resolved-user.png)

## Security Monitoring SIEM (Wazuh)
![Wazuh Failed Login](screenshots/wazuh-failed-login-4625.png)
![Account Lockout](screenshots/wazuh-account-lockout-4740.png)
![Privilege Escalation](screenshots/wazuh-privilege-escalation-4732.png)

## Lessons Learned
- Importance of time synchronization for log analysis
- Troubleshooting DNS and network connectivity issues
- Managing endpoint security agents
- Following least privilege principles
- Documenting incidents and resolutions

## Future Improvements
- Integrate vulnerability scanning
- Build custom Wazuh dashboards
- Add cloud-based monitoring
- Automate deployment with scripts
