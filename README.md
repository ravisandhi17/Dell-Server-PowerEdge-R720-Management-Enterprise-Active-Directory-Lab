# Dell Server Management & Enterprise Active Directory Lab

## Project Overview

This project demonstrates a complete **Enterprise IT Infrastructure Lab** built using:

- Windows Server (Dell PowerEdge R720 with iDRAC management)

- Windows 11 Client VM (Oracle VirtualBox)

- Active Directory Domain Services (AD DS)

- Group Policy Objects (GPO)

- Remote Server Administration (RDP + iDRAC Virtual Console)

The environment simulates real-world corporate IT administration including identity management, system control, and remote server operations.

---

## Objectives

- Deploy and configure Active Directory Domain Services (AD DS)

- Create and manage Organizational Units (OUs)

- Implement domain user management

- Apply Group Policy Objects (GPO)

- Enforce role-based access control (RBAC)

- Simulate enterprise IT department structure

- Manage Dell server using iDRAC and Virtual Console

- Enable Remote Desktop administration from client VM

---

##  Lab Architecture

###  Server (Domain Controller)

- Windows Server running on Dell PowerEdge hardware

- Domain Name: `ravikumar.local`

- DNS integrated with Active Directory

###  Client Machine

- Windows 11 VM (Oracle VirtualBox)

- Joined to domain: `ravikumar.local`

---

##  Active Directory Structure

### Organizational Units (OUs)

- IT_DELL

- HR_DELL

- SALES_DELL

### Users Created

- ITDELLUSER1 → IT_DELL

- HRDELLUSER1 → HR_DELL

- SALESDELLUSER1 → SALES_DELL

---

##  Group Policy Configuration

###  IT Department (Full Access)

- Control Panel: Enabled

- Command Prompt: Enabled

- Full administrative-style access

###  HR Department (Restricted Access)


- Control Panel: Disabled

- Command Prompt: Disabled

- Highly restricted system access for security compliance

###  SALES Department (Standard Access)

- Control Panel: Disabled

- Command Prompt: Enabled

- Balanced user environment for business operations

---

##  Server Management (Dell iDRAC)

The Dell PowerEdge server was managed using **iDRAC (Integrated Dell Remote Access Controller)** for out-of-band hardware administration.

### Features used:

- Remote power control (ON/OFF/Reset)

- Hardware monitoring (CPU, RAM, storage status)

- BIOS-level configuration access

- Server health monitoring

---

##  Virtual Console (iDRAC)

The iDRAC Virtual Console was used to access the server screen remotely.

### Capabilities demonstrated:

- Full remote GUI access to Windows Server

- BIOS and boot process monitoring

- Troubleshooting startup issues

- Remote installation and configuration support

---

## Remote Desktop (RDP)

Remote Desktop Protocol (RDP) was enabled for OS-level server management.

### Configuration:

- RDP enabled on Windows Server

- Firewall configured for remote access

- Administrator login used for testing

### Testing:

- Successfully connected from Windows 11 VM using `mstsc`

- Full GUI-based server administration achieved remotely

---

## Technologies Used

- Windows Server (Active Directory, DNS)

- Windows 11 VM

- Oracle VM VirtualBox

- Dell iDRAC Management Interface

- Group Policy Management Console (GPMC)

- Active Directory Users and Computers (ADUC)

- Remote Desktop Protocol (RDP)

- TCP/IP Networking

---

##  Testing Performed

- Domain join verification (`ravikumar.local`)

- User login testing across all departments

- GPO enforcement validation using `gpupdate /force`

- Control Panel and CMD restriction testing

- Remote Desktop connectivity test

- iDRAC Virtual Console access validation

---

##  Key Results

✔ Fully functional Active Directory domain environment  

✔ Multi-department OU structure implemented  

✔ Role-based access control (RBAC) successfully configured  

✔ Centralized policy enforcement using GPO  

✔ Dell server managed using iDRAC (enterprise-level skill)  

✔ Remote administration via RDP and Virtual Console  

✔ Enterprise-style IT infrastructure successfully simulated  

---

##  What This Project Demonstrates

This lab simulates real-world enterprise IT infrastructure including:

- Active Directory identity management

- Centralized system control using Group Policy

- Role-based security enforcement

- Server hardware management (iDRAC)

- Remote system administration (RDP + Virtual Console)

- Client-server architecture in a virtual environment

---

##  Future Enhancements

- Add second Domain Controller (redundancy setup)

- Configure Windows DHCP Server

- Implement file server with NTFS permissions

- Deploy software via Group Policy (MSI deployment)

- Configure roaming profiles and folder redirection

- Enable Windows Server backup and recovery

- Add multiple client VMs for scalability testing

---

##  Author

Ravi Kumar  

Server Management & Enterprise Active Directory Lab
