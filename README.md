# Virtual-Network
A team project developed at Babeș-Bolyai University, as part of the Operating Systems class, where we managed to connect 3 virtual machines between them.

## 📑 Table of Contents
- [Overview](#overview)
- [Technologies and Tools](#technologies-and-tools)
- [Architecture](#architecture)
- [Implementation Details](#implementation-details)
- [Testing and Validation](#testing-and-validation)
- [Security Configuration](#security-configuration)
- [Documentation](#documentation)
- [Learning Outcomes](#learning-outcomes)

---

## Overview
This project demonstrates the design and implementation of a **hybrid virtual network** integrating both Windows and Linux environments.  
The setup includes three virtual machines:

- **Windows Server (Domain Controller)**
- **Windows 10 Client**
- **Ubuntu Server**

The objective was to simulate a small enterprise network with centralized authentication, network services, web hosting, email functionality, and file sharing.  
This work was completed as a **team project** for the Operating Systems course.

---

## Technologies and Tools

### Operating Systems:
- Windows Server
- Windows 10
- Ubuntu Server

### Network and Directory Services:
- Active Directory (AD)
- DNS
- DHCP
- Group Policy (GPO)

### Web and Mail Services:
- Apache
- Nginx
- Postfix
- Dovecot
- Roundcube (Webmail)

### File Sharing:
- Samba (SMB protocol)
- NFS

### Security and Access:
- HTTPS (SSL Certificates)
- Firewall Configuration
- SSH and SFTP Access

## Architecture
The network consists of:

 - A Windows Server acting as the Domain Controller and DNS/DHCP provider.
 - A Windows 10 Client joined to the domain, managed via Group Policy.
 - An Ubuntu Server hosting web (Apache/Nginx), mail (Postfix/Dovecot), and file transfer (SFTP/Samba) services.
This setup enables domain authentication, internal name resolution, shared storage, and secure communication between Windows and Linux systems.

## Implementation Details
Configured and deployed core services: Active Directory, DNS, DHCP, GPO, Apache, Nginx, Postfix, Dovecot, Samba, SFTP.
Implemented user management and permissions through AD and Linux group policies.
Integrated Windows and Linux services for seamless interoperability.
Created startup scripts and documentation for reproducible setup.

## Testing and Validation
Comprehensive testing was conducted to verify:

 - Domain integration between Windows 10 and Windows Server
 - Access control and file sharing permissions via Samba and AD users
 - Web and mail service availability under different configurations
 - Cross-platform connectivity through SSH and SFTP

## Security Configuration
 - Applied Windows Firewall rules for essential ports and service isolation.
 - Configured Linux ufw / iptables for network-level security and access restriction.
 - Enabled encrypted connections via HTTPS and SSH.
 - Enforced strong authentication policies through AD and Linux user controls.

## Documentation
A detailed technical report was written, including:

 - System architecture diagrams
 - Step-by-step configuration procedures
 - Troubleshooting methods
 - Test results and verification logs

## Learning Outcomes
This project demonstrates:

 - Practical implementation of enterprise-level networking concepts
 - System administration across Windows and Linux environments
 - Application of virtualization, security, and network configuration principles
 - Documentation and teamwork in a technical environment

