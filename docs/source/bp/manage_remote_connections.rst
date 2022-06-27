..
  Created by: mike garcia
  To: BP for managing remote connections, largely from 12-11-2020 spotlight

.. |bp_title| replace:: Managing Remote Connections

|bp_title|
----------------------------------------------

Remote or traveling employees often require access to enterprise data while physically outside of the workplace. This can be accomplished via Virtual Private Networks (VPNs). Other common uses include securely connecting on public Wi-Fi, user anonymity, and circumventing government censorship.

VPNs encrypt and transmit data, allowing a user to securely connect to the internet or access a remote network on an untrusted connection. This ensures that all transmitted data remains confidential. Organizations need to authenticate the device or user attempting to establish a VPN connection before allowing them access. VPNs can also be used to establish secure connections between two organizations on separate networks.

Many cybersecurity firms offer ready-made hardware and software solutions to deploy a VPN. Well-resourced organizations can also develop their own solutions, such as setting up a VPN router to manage secure connections.

Employees can connect to VPNs via laptops, desktops, or even mobile devices such as smartphones and tablets. When an employee connects to a VPN, it will appear as if they are connecting to the internet from the organization’s network, instead of their remote location. Below is a diagram showing how VPNs may be used in an election system.

.. image:: /_static/VPN.png
  :width: 90%
  :alt: Virtual Private Network Diagram

Election offices can use a VPN to:

* Protect employee data if a remote or offsite employee must connect to an office network, or transmit sensitive data (e.g., employee or election data).
* Securely connect local election officials’ workstations to a state voter registration database.
* Securely transmit information to an external partner, such as an election vendor or non-profit organization.

Goals
**********************************************

#. Understand VPN technology and its role in election environments (|Maturity1| maturity)
#. Properly implement a VPN service with your environment (|Maturity1| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _manage-remote-connections-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

At the |Maturity1| maturity, organizations should use a VPN for all remote connections. To do so:

#. Recognize situations where a VPN would be useful and appropriate.
#. Implement multi-factor authentication on all VPN connections.
#. Review CIS’s `Telework and Small Office Network Security Guide <https://www.cisecurity.org/insights/white-papers/cis-controls-telework-and-small-office-network-security-guide>`_ for tips on securing a remote work environment.
#. If a trusted third party, like a vendor, provides the VPN used to connect to your network, confirm they are following the same security principles as your organization.

.. _manage-remote-connections-maturity-two-three:

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

In addition to the actions at the |Maturity1| maturity, at the |Maturity2| maturity, you should also:

#. Update the hardware and software used by VPNs and implement a patch management program to prevent malicious actors from exploiting known vulnerabilities. There have been reports of cyber threat actors targeting VPNs by exploiting known vulnerabilities in hardware/software systems.
   * For example, see examples of Common Vulnerabilities and Exposures (:term:`CVE`) :ref:`here <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2018-13379>`_ and :ref:`here <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-11510>`_, that led to :ref:`this <https://www.nsa.gov/Press-Room/News-Highlights/Article/Article/2573391/russian-foreign-intelligence-service-exploiting-five-publicly-known-vulnerabili/>`_ joint advisory.
#. Review `CISA’s Enterprise VPN Security Alert <https://www.cisa.gov/uscert/ncas/alerts/aa20-073a>`_
#. Review `NIST's Guide to Enterprise Telework, Remote Access, and Bring Your Own Device (BYOD) Security <https://csrc.nist.gov/publications/detail/sp/800-46/rev-2/final>`_

Cost-Effective Tools
**********************************************

* CIS Telework and Small Office Network Security Guide: This Guide is meant to assist individuals and organizations in securing commodity routers, modems, and other network devices. Securing these devices is important as there are serious cybersecurity considerations surrounding the usage of network devices. (https://www.cisecurity.org/insights/white-papers/cis-controls-telework-and-small-office-network-security-guide)

Learn More
**********************************************

* For more tips on working with vendors, review CIS’s _`“A Guide for Ensuring Security in Election Technology Procurements.” <https://www.cisecurity.org/elections>`

Mapping to CIS Controls and Safeguards
**********************************************

* 3.10: Encrypt Sensitive Data in Transit (|Maturity1| maturity)
* 6.3: Require MFA for Externally-Exposed Applications (|Maturity1| maturity)
* 6.4: Require MFA for Remote Network Access (|Maturity1| maturity)
* 12.6: Use of Secure Network Management and Communication Protocols (|Maturity1| maturity)
* 12.7: Ensure Remote Devices Utilize a VPN and are Connecting to an Enterprise’s AAA Infrastructure (|Maturity2| maturity)

Mapping to CIS Handbook Best Practices
****************************************

* 44, 46, 83
