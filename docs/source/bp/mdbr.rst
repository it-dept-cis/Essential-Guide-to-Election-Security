..
  Created by: mike garcia
  To: MDBR based on slick sheet feb 2022

.. |bp_title| replace:: Malicious Domain Blocking and Reporting

.. admonition:: Status
   :class: caution

   Soft Launch Draft

|bp_title|
----------------------------------------------

:term:`Malicious Domain Blocking and Reporting`, or :term:`MDBR`, technology prevents IT systems from connecting to harmful web domains, helping limit infections related to known malware, ransomware, phishing, and other cyber threats. This capability can block the vast majority of ransomware infections just by preventing the initial outreach to a ransomware delivery domain.

Once an organization points its domain name system (:term:`DNS`) requests to the MDBR DNS server IP addresses, every DNS lookup will be compared against a list of known and suspected malicious domains. Attempts to access known malicious domains such as those associated with malware, phishing, and ransomware, among other threats, are blocked and logged.

.. figure:: /_static/MDBR-Simple-Secure-DNS-Diagram.22.01.png
   :width: 90%
   :alt: Graphic showing MDBR working in an election office environment

   :term:`MDBR` in an election office environment

Goals
**********************************************

#. Deploy MDBR for all internet-facing IT assets (|Maturity1| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions are the same for all maturity levels.

The EI-ISAC provides members with a free MDBR service. Members sign up and configure their DNS server, and the EI-ISAC will then provide reporting that includes log information for all blocked requests and assist in remediation if needed.

The service is easy to implement and requires virtually no maintenance as EI-ISAC and its provider fully maintain the systems required to provide the service.

The EI-ISAC hosts all reporting data, including both successful and blocked DNS requests. It will then perform detailed analysis and reporting for the organization and the election community writ large. The EI-ISAC will provide regular reporting and intelligence services for SLTT members.

* If you're an EI-ISAC member, you can sign up for no-cost MDBR by registering at https://mdbr.cisecurity.org. You will be asked to provide the following information:

  * Your contact information
  * Technical contact(s) for MDBR setup, troubleshooting, and general technical support
  * Reporting contact(s) for receiving reports on your MDBR service
  * Public IP addresses or CIDR netblocks from which your organization’s DNS queries are sent

* If you aren't an MS-ISAC or EI-ISAC member, _`join today <join_ei_isac>`!

Cost-Effective Tools
**********************************************

* EI-ISAC MDBR service: A no-cost, lightweight MDBR solution for EI-ISAC members [https://mdbr.cisecurity.org]

Mapping to CIS Controls and Safeguards
**********************************************

* 9.2: Use DNS Filtering Services
* 9.3: Maintain and Enforce Network-Based URL Filters

Mapping to CIS Handbook Best Practices
****************************************

* There are no relevant Handbook best practices

-----------------------------------------------
