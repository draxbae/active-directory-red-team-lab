# Active Directory Red Team Lab

Hands-on Active Directory security lab focused on reconnaissance, enumeration, and authenticated security assessment in an isolated virtual environment.

## Lab Overview

This project documents a self-contained Active Directory lab built using:

- Windows Server 2022
- Kali Linux
- VirtualBox
- Active Directory Domain Services
- NetExec
- Nmap
- PowerShell

## Lab Environment

| Component | Details |
|---|---|
| Domain Controller | AD-DC01 |
| Operating System | Windows Server 2022 |
| Domain | corp.local |
| Network | Isolated Host-only Network |
| Client | Kali Linux |

## Objectives

- Build a functional Active Directory environment
- Understand basic Windows domain architecture
- Perform network and service enumeration
- Identify common AD-related services
- Perform authenticated SMB and LDAP enumeration
- Practice security assessment methodology in a controlled lab

## Methodology

### 1. Active Directory Setup

Configured Windows Server 2022 as an Active Directory Domain Controller and created the `corp.local` domain.

### 2. Network Verification

Verified connectivity between Kali Linux and the Domain Controller using ICMP and DNS queries.

### 3. Service Enumeration

Used Nmap to identify exposed services commonly associated with Active Directory, including:

- DNS
- Kerberos
- LDAP
- SMB
- RPC
- Global Catalog

### 4. Authenticated SMB Assessment

Used NetExec with a dedicated lab account to verify authenticated access and enumerate available SMB shares.

### 5. LDAP Enumeration

Performed authenticated LDAP enumeration to identify domain users and groups.

### 6. User Enumeration

Identified the following default and lab accounts:

- Administrator
- Guest
- krbtgt
- labuser

## Tools Used

- Nmap
- NetExec
- PowerShell
- Active Directory PowerShell Module
- VirtualBox
- Kali Linux
- Windows Server 2022

## Key Learning Outcomes

- Active Directory domain fundamentals
- Windows authentication concepts
- SMB enumeration
- LDAP enumeration
- Kerberos service identification
- Domain user and group enumeration
- Basic Red Team reconnaissance methodology

## Security Notes

This project was performed entirely inside an isolated virtual lab created for educational purposes.

No real-world systems, accounts, or unauthorized infrastructure were targeted.

Sensitive credentials, detailed exploitation procedures, and unnecessary infrastructure information are intentionally excluded from this repository.

## Project Status

### Completed

- [x] Active Directory Domain Controller
- [x] Domain configuration
- [x] Kali-to-DC connectivity
- [x] DNS verification
- [x] Nmap service enumeration
- [x] SMB enumeration
- [x] LDAP enumeration
- [x] Domain user enumeration
- [x] Group enumeration

### Future Improvements

- [ ] Add Windows client machine
- [ ] Create additional security misconfiguration scenarios
- [ ] Perform controlled privilege escalation exercises
- [ ] Document detection and mitigation techniques

## Disclaimer

This repository is a learning project demonstrating Active Directory security assessment techniques in an authorized laboratory environment.
