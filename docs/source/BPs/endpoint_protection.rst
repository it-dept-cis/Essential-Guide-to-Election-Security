..
  Created by: mike garcia
  To: end point protection, EDR, etc.

.. |bp_title| replace:: Endpoint Protection

|bp_title|
----------------------------------------------

:term:`Endpoint protection` is security software that is deployed on workstations and servers, which are commonly referred to as “endpoints.” A common name for this is :term:`Endpoint Detection and Response`, or EDR. EDR collects technical data from these endpoints and transmits it back to the vendor or a local server. The data is then analyzed for suspicious patterns and threats.

If a threat is identified, it is blocked and an alert is generated. Administrators can typically view alerts through a vendor control panel or a connection to their own security platform. Also, many EDR solutions include a traditional antivirus functionality and the ability for responders to remotely access compromised systems for remediation.

.. include:: ../_static/EDR-Vendor-Cloud-Diagram-v21.01.png

Election offices can use EDR to:

* Detect and stop active attacks on election infrastructure,
* Protect against malware,
* Quarantine suspicious files,
* Isolate compromised systems,
* Remediate malware infections,
* Enable analysis to find and mitigate threats, and
* Disable and restrict the ability of suspicious users on your network to cause harm.

Goals
**********************************************

#.  Understand EDR technology and why it's important
#.  Know how to get EDR services through the EI-ISAC or commercial vendors

Mappings to CIS Controls and Safeguards
**********************************************

* 10.1: Deploy and Maintain Anti-Malware Software
* 10.6: Centrally Manage Anti-Malware Software

Actions
**********************************************

The EI-ISAC offers EDR services at no charge to state and local election offices. Election offices should contact the |eiisac_email| for more information.

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#.  Deploy EDR on systems throughout your network.
    * All your systems and endpoints that touch the elections processes are covered at no cost to you by the federally-funded EDR program. Additionally, your jurisdiction’s non-election endpoints can also sign up for the same services at a discounted cost. Contact the |eiisac_email| for more information.
    * You may also review CIS's _`Guide for Ensuring Security in Election Technology Procurements <https://www.cisecurity.org/elections>` for best practices in crafting proposals and other necessary documents.
#.  Take advantage of vendor-offered user training for usage of EDR tools.
#.  Implement best practices for EDR:
    * Delegate personnel to monitor and act on detections.
    * Export information regularly from the control panel to local hardware backups, so you always have access to data needed for audits and investigations.
    * Consider available staffing resources to support any new security infrastructure and the associated responsibilities. Many EDR providers offer solutions supported by a 24×7 team to manage and respond to identified incidents.
    * Refer to the _`EI-ISAC Cyber Incident Checklist <https://www.cisecurity.org/insights/white-papers/cyber-incident-checklist>` to manage security events.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For the |Maturity2| and |Maturity3| maturities, all of the guidance for the |Maturity1| maturity applies, but the specifics of your network configuration and the number of endpoints you serve may affect whether you can implement EDR through the EI-ISAC. Contact the |eiisac_email| for more information.

Cost-Effective Tools
**********************************************

*   EI-ISAC EDR program: EDR services at no charge to state and local election offices. (Contact |eiisac_email|)

Learn More
**********************************************

*   :doc:`EI-ISAC EDR program brochure <../_static/EI-ISAC EDR Overview Online.22.01.pdf>`

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |eges_email|.
