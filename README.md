# Active Directory Enviroment attack


This project involved setting up an Active Directory environment on a Proxmox server with a Windows 2022 Domain Controller and a Windows 10 workstation. The objective was to deliberately test and identify vulnerabilities within the Active Directory infrastructure.

After configuring the Active Directory, I ran a script to increase the Domain Controller's susceptibility to vulnerabilities, allowing for controlled security testing.

Utilizing tools such as 'Kerbrute' in Kali Linux, the project successfully identified potential security gaps by retrieving user credentials from the Domain Controller.

Incorporating Mythic as a command-and-control framework(C2), tools like BloodHound and SharpHound were used to gather critical data from the Domain Controller. This data was then analyzed in BloodHound to uncover vulnerabilities and potential points of exploitation.
