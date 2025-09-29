# Windows & Network Services Project

[![Windows Server](https://img.shields.io/badge/Windows-Server-0078D6?logo=windows&logoColor=white)](https://learn.microsoft.com/en-us/windows-server/)
[![Active Directory](https://img.shields.io/badge/Active%20Directory-Identity-blue)](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
[![Status](https://img.shields.io/badge/Status-Learning-green)]()
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)]()

A hands-on project covering **Windows Server Active Directory** and essential **network services**.
Includes domain setup, AD management, NAT, DNS, DHCP, RDP, FTPS, MySQL, and Group Policy software deployment.

---

## Network & Domain Topology

```sh
                    ┌───────────────┐
                    │     WAN       │
                    │   Internet    │
                    └───────┬───────┘
                            │
                     ┌──────▼──────┐
                     │  Windows DC  │
                     │ (AD, DNS,    │
                     │  DHCP, GPO)  │
                     └──────┬──────┘
        ┌───────────────┼───────────────┐
        │               │               │
 ┌──────▼──────┐  ┌─────▼──────┐  ┌─────▼─────┐
 │ Windows 10  │  │ File/FTPS  │  │ MySQL      │
 │ Domain User │  │  Server    │  │ Server     │
 └─────────────┘  └────────────┘  └────────────┘
```

---

## Tasks

1. `Task01` -> Configure LAN, WAN, NAT & Internal Network
2. `Task02` -> Promote to Domain Controller & Join Windows 10 to the Domain
3. `Task03` -> Users, Groups, and Organizational Units in Active Directory
4. `Task04` -> Shared Resources: SMB & Printers in Windows-AD
5. `Task05` -> SNAT, Routing & Network Configuration
6. `Task06` -> DNS - Domain Name System
7. `Task07` -> DHCP - Dynamic Host Configuration Protocol
8. `Task08` -> RDP - Remote Desktop Protocol
9. `Task09` -> FTPS - File Transfer Protocol Secure
10. `Task10` -> HTTP & HTTPS
11. `Task11` -> MySQL: Workbench, Shell, Server & Winget
12. `Task12` -> GPO: Software Installation & Deployment via Group Policy

---

## Quick Start

1. Set up a virtualization platform (VirtualBox / VMware / Proxmox).
2. Install **Windows Server (2019/2022/2025)** and **Windows 10 client**.
3. Follow each task in order to build a complete domain + network services environment.

---

## References

- [Active Directory Docs](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [DNS Server Docs](https://learn.microsoft.com/en-us/windows-server/networking/dns/dns-top)
- [DHCP Server Docs](https://learn.microsoft.com/en-us/windows-server/networking/technologies/dhcp/dhcp-top)
- [Group Policy Docs](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/group-policy)
- [MySQL Documentation](https://dev.mysql.com/doc/)

---

## Author

**thierno953** - System & Network Administration | Active Directory | Cybersecurity Enthusiast
