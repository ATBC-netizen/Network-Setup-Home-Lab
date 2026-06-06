# Mock Enterprise Network Setup

## Objective
The goal of this project was to design, deploy, and manage a network with infrastructure comprising Active Directory Domain Services (AD/DS), Domain Name System (DNS), and Dynamic Host Configuration Protocol (DHCP).

## Lab Architecture & IP Addressing
* **Network ID:** `192.168.1.0`
* **Domain Controller / DNS Server:** `192.168.1.50` (Windows Server 2022 Datacenter Edition - Desktop Experience)
* **DHCP Server:** `192.168.1.49` (Windows Server 2022 Datacenter Edition - Server Core)
* **Client Workstation:** `192.168.1.51` (DHCP Leased - Windows 11 Enterprise)
* **Domain Name:** `SERVER-LAB.local`

---

## 1. Directory Architecture
<img width="559" height="391" alt="Architecture (OUs)" src="https://github.com/user-attachments/assets/a2c72121-5e2a-4818-9922-789cdca33292" />

**Figure 1: Active Directory Enterprise Hierarchy** 

Designed a secure Organisational Unit (OU) hierarchy to isolate privileged accounts from standard users, workstations, and network infrastructure, facilitating strict Role-Based Access Control (RBAC) through Group Policy Objects (GPOs).

## 2. Dynamic Host Configuration Protocol Setup
<img width="755" height="221" alt="DHCP Setup (Core)" src="https://github.com/user-attachments/assets/81d5ab1e-b5bd-4312-a866-1b631dae6842" />

**Figure 2: Deploying DHCP on Server Core** 

Deployed an authorised Windows Server Core instance to act as the primary DHCP server for the `SERVER-LAB.local` network using native PowerShell cmdlets. Windows Server Core was utilised to significantly reduce the attack surface and the operating system's footprint. 

## 3. Remote Administration (RSAT)
<img width="485" height="197" alt="RSAT Setup (DC)" src="https://github.com/user-attachments/assets/6b1e479e-0a07-4e2a-87d3-7000fa41960d" />

**Figure 3: Centralised Management of Network Infrastructure**

Utilised Remote Server Administration Tools (RSAT) on the Domain Controller to centralise the management of network infrastructure with a Graphical User Interface (GUI). Enabling the remote management of DHCP from the linked Server Core instance responsible for DHCP at `192.168.1.49`.

## 4.
<img width="443" height="461" alt="W11 ipconfig" src="https://github.com/user-attachments/assets/32f8dfba-9411-4069-b721-f8c19e37b744" />

**Figure 4: INCOMPLETE**

---

## Challenges & Learning Process
