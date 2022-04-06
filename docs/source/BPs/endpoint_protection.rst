..
  Created by: mike garcia
  To: end point protection, EDR, etc.

.. |bp_title| replace:: Endpoint Protection

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

:term:`Endpoint Protection` is security software that is deployed on workstations and servers, which are commonly referred to as “endpoints.” A common name for this is :term:`Endpoint Detection and Response`, or EDR. EDR collects technical data from these endpoints and transmits it back to the vendor or a local server. The data is then analyzed for suspicious patterns and threats.

If a threat is identified, it is blocked and an alert is generated. Administrators can typically view alerts through a vendor control panel or a connection to their own security platform. Also, many EDR solutions include a traditional antivirus functionality and the ability for responders to remotely access compromised systems for remediation.

.. include:: EDR-Vendor-Cloud-Diagram-v21.01.png

Election offices can use EDR to:
* Detect and stop active attacks on election infrastructure.
* Protect against malware.
* Disable and restrict the ability of suspicious users on your network to cause harm.

Goals
**********************************************

#.	Understand EDR technology and why its important
#.	Know how to get EDR services through the EI-ISAC or commercial vendors

Mappings to CIS Controls and Safeguards
**********************************************

- [10.1][tab] Deploy and Maintain Anti-Malware Software
- [10.6][tab] Centrally Manage Anti-Malware Software

Actions
**********************************************

The EI-ISAC offers free EDR services for a limited number of endpoints. Election offices should contact the |eiisac_email| for more information.

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

 At the |Maturity1| maturity, you should consider deploying EDR across all endpoints in your environment.

* Deploy EDR on systems throughout your network.
  - Depending on the number of endpoints you have and relationship with other non-election local entities--like county recorder--you may be able to have your all of your endpoints covered by the EI-ISAC.
  - Otherwise, review the CIS Guide for Ensuring Security in Election Technology Procurements for best practices in crafting proposals and other necessary documents.
* Implement best practices for EDR:
  - Take advantage of vendor-offered user training.
  - Delegate personnel to monitor and act on detections.
  - Export information regularly from the control panel to local hardware backups, so you always have access to data needed for audits and investigations.
  - Consider available staffing resources to support any new security infrastructure and the associated responsibilities. Many EDR providers offer solutions supported by a 24×7 team to manage and respond to identified incidents.
  - Refer to the _`EI-ISAC Cyber Incident Checklist <https://www.cisecurity.org/insights/white-papers/cyber-incident-checklist>` to manage security events.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For the |Maturity2| and |Maturity3| maturities, all of the guidance for the |Maturity1| maturity applies, but the specifics of your network configuration and the number of endpoints you serve may affect whether you can implement EDR through the EI-ISAC. Contact the |eiisac_email| for more information.


Cost-Effective Tools
**********************************************

•	[tool]: [description][(link)]
•	[tool]: [description][(link)]

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************
•	[links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |contact_email|.

This page last updated on |last_update|.
