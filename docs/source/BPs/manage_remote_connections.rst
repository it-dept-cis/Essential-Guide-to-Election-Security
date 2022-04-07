..
  Created by: mike garcia
  To: BP for managing remote connections, largely from 12-11-2020 spotlight

.. |bp_title| replace:: Managing Remote Connections

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Virtual Private Networks (VPNs) encrypt and transmit data allowing a user to securely connect to the internet or access a remote network on an untrusted connection. This ensures that all transmitted data remains confidential.

Organizations use VPNs to allow employees to connect to their internal network when working remotely. Other common uses include securely connecting on public Wi-Fi, user anonymity, and circumventing government censorship. Many cybersecurity firms offer ready-made hardware and software solutions to deploy a VPN. Well-resourced organizations can also develop their own solutions, such as setting up a VPN router to manage secure connections.

When an employee connects to a VPN, it will appear as if they are connecting to the internet from the organization’s network, instead of their remote location. Below is a diagram showing how VPNs may be used in an election system.

.. include:: VPN.png

Election offices can use a VPN to:

* Protect data streams if a remote or offisite employee must connect to an office network, or transmit sensitive data (e.g. employee or election data).
* Securely connect local election officials’ workstations to a state voter registration database.
* Securely transmit information to an external partner, such as an election vendor.
* Use secure network management and communication protocols (e.g., 802.1X, Wi-Fi Protected Access 2 (WPA2)
Enterprise or greater).

* NEED TO DISCUSS AUTHENTICATION *
* NEED TO CHANGE TITLE OF BP TO SECURE NETWORK TRAFFIC or something *

Goals
**********************************************

#.	Understand VPN technology and its role in election environments
#.	Know how to properly implement a VPN service with your environment

Mappings to CIS Controls and Safeguards
**********************************************

- [3.10][tab][Encrypt Sensitive Data in Transit]
- [12.6][tab][Use of Secure Network Management and Communication Protocols]
- [12.7][tab][Ensure Remote Devices Utilize a VPN and are Connecting to an Enterprise’s AAA Infrastructure]

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

At the |Maturity1| maturity, organizations should use a VPN for all remote connections. To do so:

*	Implement multi-factor authentication on all VPN connections.
*	Review CIS’s “Telework and Small Office Network Security Guide” for tips on securing a remote work setup.
* If a trusted third party, like a vendor, provides the VPN used to connect to your network, confirm they are following the same security principles as your organization.
  * For more tips on working with vendors, review CIS’s _`“A Guide for Ensuring Security in Election Technology Procurements.” <https://www.cisecurity.org/elections>`

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

In addition to the actions at the |Maturity1| maturity, at the |Maturity2| maturity, you should also:

* Update the hardware and software used by VPNs and implement a patch management program to prevent malicious actors from exploiting known vulnerabilities. There have been reports of cyber threat actors targeting VPNs by exploiting known vulnerabilities in hardware/software systems.
* Review _`CISA’s Enterprise VPN Security Alert <https://www.cisa.gov/uscert/ncas/alerts/aa20-073a>`
* Review _`NIST's Guide to Enterprise Telework, Remote Access, and Bring Your Own Device (BYOD) Security <https://csrc.nist.gov/publications/detail/sp/800-46/rev-2/final>`

Cost-Effective Tools
**********************************************

•	[CIS Telework and Small Office Network Security Guide]: [This Guide is meant to assist individuals and organizations in securing commodity routers, modems, and other network devices. Securing these devices is important as there are serious cybersecurity considerations surrounding the usage of network devices.][(https://www.cisecurity.org/insights/white-papers/cis-controls-telework-and-small-office-network-security-guide)]

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************
•	[links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |contact_email|.

This page last updated on |last_update|.
