# Active Directory Enviroment attack


This project involved setting up an Active Directory environment on a Proxmox server with a Windows 2022 Domain Controller and a Windows 10 workstation. The objective was to deliberately test and identify vulnerabilities within the Active Directory infrastructure.

After configuring the Active Directory, I ran a script to increase the Domain Controller's susceptibility to vulnerabilities, allowing for controlled security testing.

Utilizing tools such as 'Kerbrute' in Kali Linux, the project successfully identified potential security gaps by retrieving user credentials from the Domain Controller.

Incorporating Mythic as a command-and-control framework(C2), tools like BloodHound and SharpHound were used to gather critical data from the Domain Controller. This data was then analyzed in BloodHound to uncover vulnerabilities and potential points of exploitation.


# Infrastructure Setup:

1. **Choice of Virtualization Platform:** You can establish the Active Directory environment using various platforms like VirtualBox, VMware, or, in this case, Proxmox. I used a Proxmox server for the setup.
2. **Components:** Deploy a Windows 2022 Domain Controller and a Windows 10 workstation.

# Configuring Active Directory:

1. **Domain Controller Configuration:** Start by installing Active Directory Domain Services on the Windows Server through Server Manager. Set up a new forest and define a root domain name.
2. **Workstation Connection:** Configure the Windows 10 workstation to connect to the Active Directory environment.

# Intentionally Making the Domain Controller Vulnerable:

The setup involves implementing controlled vulnerabilities within the Domain Controller to examine its susceptibility to various attacks and security breaches.

1. **Vulnerability Script:** A script from a specified GitHub repository (link provided below) is used to increase the vulnerabilities within the Domain Controller environment.
2. **Testing for Weaknesses:** Employ tools to discover and exploit potential security gaps, focusing on retrieving user credentials from the Domain Controller.

# Exploiting Vulnerabilities:

Exploration of vulnerabilities is critical to understand how security breaches might occur within an Active Directory environment.

1. **Kerbrute Enumeration:** Utilize Kerbrute to perform user enumeration and attempt to identify passwords associated with user accounts.
2. **Password Testing:** Use the discovered credentials to authenticate services and access user accounts.

# Post-Exploitation Activities:

This phase involves utilizing the gained access to further exploit the environment and maintain control:

1. **Tools for Control:** Employ specific tools like 'evil-winrm' to establish connections and control the compromised accounts.
2. **Utilizing Mythic:** Deploy the Mythic framework to create payloads and maintain access through a stable connection.
3. **Analyzing Active Directory with BloodHound:** Employ BloodHound and SharpHound tools to extract and analyze comprehensive information, uncovering intricate details about the Active Directory environment.


