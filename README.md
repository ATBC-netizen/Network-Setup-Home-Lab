# Mock Enterprise Network Setup

## Objective
The goal of this home lab was to design, deploy, and manage a network infrastructure comprising Active Directory Domain Services (AD/DS), Domain Name System (DNS), and Dynamic Host Configuration Protocol (DHCP).

## Lab Architecture & IP Addressing
* **Network ID:** `192.168.1.0`
* **Domain Controller / DNS Server:** `192.168.1.50` (Windows Server 2022 Datacenter Edition - Desktop Experience)
* **DHCP Server:** `192.168.1.49` (Windows Server 2022 Datacenter Edition - Server Core)
* **Client Workstation:** `192.168.1.51` (DHCP Leased - Windows 11 Enterprise)
* **Domain Name:** `SERVER-LAB.local`

---

## 1. Directory Architecture
<img width="559" height="391" alt="Architecture (OUs)" src="https://github.com/user-attachments/assets/a2c72121-5e2a-4818-9922-789cdca33292" />
**Figure 1: Active Directory Enterprise Hierarchy** Designed a secure Organisational Unit (OU) hierarchy to isolate privileged accounts from standard users, workstations, and network infrastructure, thus facilitating strict Role-Based Access Control (RBAC) through Group Policy Objects (GPOs).

## 2. 

## 3.

## 4.

---

## Challenges & Learning Process


<img width="755" height="221" alt="DHCP Setup (Core)" src="https://github.com/user-attachments/assets/81d5ab1e-b5bd-4312-a866-1b631dae6842" />

<img width="1129" height="291" alt="DHCP Address Leases" src="https://github.com/user-attachments/assets/21a3ef6e-ef9a-4051-98db-be120bc6db9e" />

<img width="443" height="461" alt="W11 ipconfig" src="https://github.com/user-attachments/assets/32f8dfba-9411-4069-b721-f8c19e37b744" />

<img width="485" height="197" alt="RSAT Setup (DC)" src="https://github.com/user-attachments/assets/6b1e479e-0a07-4e2a-87d3-7000fa41960d" />
