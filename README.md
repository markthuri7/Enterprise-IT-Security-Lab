# Enterprise IT & Security Home Lab

## Overview
This project documents a Windows enterprise lab environment built to practice IT support and cybersecurity operations.

The lab simulates a corporate network with centralized authentication, endpoint management, and security monitoring.

## Technologies Used
- Windows Server 2022 (Domain Controller)
- Active Directory & DNS
- Windows 11 Pro Client
- VirtualBox
- Internal Network (LabNet)

## Lab Architecture
- DC01 (192.168.100.10) – Domain Controller, DNS
- PC01 (192.168.100.20) – Domain Client
- Domain: lab.local

## Key Skills Demonstrated
- Installed and configured Active Directory Domain Services
- Created and managed domain users
- Joined Windows clients to domain
- Configured DNS and static IPs
- Troubleshot connectivity and authentication issues
- Implemented Group Policy to enforce automatic screen lock and password protection
- Verified policy deployment using gpresult and gpupdate

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

## Future Enhancements
- SIEM integration
- Ticketing system
- Endpoint protection
- Cloud integration
