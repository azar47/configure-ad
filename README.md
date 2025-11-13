# On-Premises Active Directory Deployment in Azure

## Project Summary
This project demonstrates the deployment and configuration of an **on-premises Active Directory (AD)** environment within **Microsoft Azure Virtual Machines**.  
The project shows how to set up a Domain Controller (DC), join a client VM to the domain, manage users and Organizational Units (OUs), and configure administrative and non-administrative accounts.

**Environments and Technologies Used:**
- **Environments:** Microsoft Azure (Virtual Machines/Compute), Remote Desktop  
- **Operating Systems:** Windows Server 2022, Windows 10 (21H2)  
- **Technologies/Applications:** Active Directory Domain Services, PowerShell  

The purpose of this project is to illustrate practical AD administration skills in a cloud-hosted environment.

## Media

<img src="<img width="1851" height="834" alt="dP825Zj" src="https://github.com/user-attachments/assets/28d6641d-b82d-4809-9760-4505f5b1e1b1" />
- **Screenshot 1:** DC-1 VM dashboard in Azure showing the Windows Server 2022 instance.

- <img src="<img width="907" height="527" alt="image2" src="https://github.com/user-attachments/assets/6f51bc53-2032-4355-a600-8fc0875a42c5" />
- **Screenshot 2:** Active Directory Users and Computers (ADUC) showing Organizational Units (_EMPLOYEES, _ADMINS, _CLIENTS).

-<img src="https://i.imgur.com/SrcGUxB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
- **Screenshot 3:** Domain Admin account (jane_admin) created and added to Domain Admins group.

-<img src="https://imgur.com/a/pToFTqF" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- **Screenshot 4:** Client-1 VM joined to the domain, visible in ADUC.  
- **Screenshot 5:** PowerShell script creating multiple user accounts and results in ADUC.  

*(Optional: more screenshots showing Remote Desktop setup, account lockout testing, and enabling/disabling accounts.)*

## Demonstration
1. Deployed two Azure VMs: **DC-1** (Domain Controller) and **Client-1** (Windows 10 client).  
2. Installed Active Directory Domain Services on DC-1 and created a new forest (`mydomain.com`).  
3. Created OUs and administrative accounts in ADUC, including `jane_admin` as a Domain Admin.  
4. Joined Client-1 to the domain and verified the computer in ADUC.  
5. Configured Remote Desktop access for non-administrative users.  
6. Created multiple additional users via PowerShell, observed accounts in the proper OUs, and tested logins on Client-1.  
7. Tested account lockout policies and enabling/disabling user accounts, observing expected behavior on both DC-1 and Client-1.  

This project demonstrates practical Active Directory administration skills, including VM setup, domain management, user management, and basic security operations.
