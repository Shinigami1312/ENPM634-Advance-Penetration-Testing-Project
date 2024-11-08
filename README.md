# ENPM634 Network Penetration Testing Project

## Overview

This repository contains the final penetration test report for ENPM634, focusing on identifying the true identity of the "Masked DJ" by exploring vulnerabilities in their IT environment. The project involved network scanning, exploitation of various systems, and retrieval of sensitive data to uncover the Masked DJ’s identity and provide security recommendations.

## Objectives

The primary goals of this assessment were to:

1. Infiltrate the Masked DJ's IT systems to discover their true identity.
2. Identify security vulnerabilities within the infrastructure, focusing on weak password management, outdated systems, and inadequate network protections.
3. Provide actionable recommendations to improve the Masked DJ's IT security.

## Methodology

The penetration test was conducted using a structured approach:

1. **Network Scanning**: Used tools like Netdiscover and Nmap to identify IP addresses and open ports of the target machines.
2. **Exploitation**: Leveraged vulnerabilities like EternalBlue on Windows 7 and SMB access on Windows Server 2016 using Metasploit.
3. **Password Cracking**: Employed John The Ripper and Hashcat to crack password hashes.
4. **Data Retrieval**: Extracted sensitive data from servers and accessed the development site to uncover the Masked DJ’s identity.

## Key Findings

- **Weak Password Policy**: Cracked passwords easily due to minimal complexity, allowing lateral movement between systems.
- **Exploitable Vulnerabilities**: Found unpatched systems susceptible to exploits such as EternalBlue.
- **Sensitive Data Exposure**: Discovered files, including "New-Password-Policy.txt" and Active Directory hashes, that revealed critical information.
- **Final Outcome**: Successfully identified the Masked DJ as young Professor Shivers after exploring the development site.

## Tools Used

- **Netdiscover & Nmap**: For network discovery and port scanning.
- **Metasploit**: To exploit vulnerabilities like EternalBlue.
- **John The Ripper & Hashcat**: For password cracking.
- **Impacket & SMBClient**: To access and retrieve files from the SMB server.
- **AWS CLI**: For downloading data from an S3 bucket linked to the target’s account.

## Challenges

1. **Password Complexity**: The password cracking process was time-consuming due to the need for various dictionaries and brute-force methods.
2. **System Navigation**: Locating the relevant files and working through limited access rights added complexity to the investigation.

## Recommendations

1. **Enhance Password Policies**: Implement complex password requirements and multi-factor authentication to prevent unauthorized access.
2. **Patch Management**: Regularly update and patch systems, especially legacy systems like Windows 7, to avoid known vulnerabilities.
3. **Network Monitoring**: Deploy intrusion detection systems (IDS) and conduct regular scans to identify unusual activity.
4. **Limit Privileges**: Apply the principle of least privilege to restrict access to sensitive data.

## Conclusion

This investigation demonstrated significant vulnerabilities within the Masked DJ’s IT infrastructure. By following our recommendations, the Masked DJ’s team can better secure their systems and prevent unauthorized access.

For detailed steps, please refer to the technical report in this repository.
