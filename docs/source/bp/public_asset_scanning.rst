..
  Created by: mike garcia
  To: network scanning to include things like CyHy

.. |bp_title| replace:: Publicly-Facing Network Scanning

*Best Practice:* |bp_title|
----------------------------------------------

All code needs to be tested for flaws, and given the types of attacks that work on a given type of code change as adversaries develop new techniques, deployed code needs to be tested regularly for known vulnerabilities.

For public-facing assets, various types of scanning can find known vulnerabilities and provide reports that prioritize them based on standardized severities. These scanning tools are automated and can run regularly to always keep you informed of your progress and any new issues due to changes you make or the evolving threat environment.

Common types of scanning or network testing include:

* Vulnerability Scanning: Reviews public-facing websites for vulnerabilities
* Web application scanning: Reviews public-facing applications for vulnerabilities
* Remote penetration testing: A more advanced method of using known tactics to simulate attacks and find more difficult to exploit vulnerabilities

Goals
**********************************************

#. Understand the types of scanning and how they can help protect publicly-facing assets
#. Know how to access free, automated services for scanning publicly-facing assets

Mappings to CIS Controls and Safeguards
**********************************************

* 7.6: Perform Automated Vulnerability Scans of Externally-Exposed Enterprise Assets
* 7.7: Remediate Detected Vulnerabilities

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Use free tools and services to conduct scans of your publicly-facing assets. This should include your website and any online portals you are responsible for that are used for elections purposes.
#. Remediate any vulnerabilities or known issues found during the scans.

Note that scanning online systems you do not own may run afoul of the Computer Fraud and Abuse Act of 1986 (:term:`CFAA`).

At the |Maturity1| maturity, you should be using free tools to conduct scanning of your publicly-facing assets.

:term:`CISA` offers all of its cybersecurity assessment services at no cost to election offices.

* Sign up for free vulnerability scanning by contacting CISA at |CISA_vuln_email| with subject line "Requesting Cyber Hygiene Services."
* If you have web applications, sign up for free web application scanning at |CISA_vuln_email| with subject line "Requesting Cyber Hygiene Services."

|Maturity2| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

At the |Maturity2| maturity, you should also implement remote penetration testing.

#. Sign up for free remote penetration testing by contacting :term:`CISA` at |CISA_vuln_email| with subject line "Requesting Cyber Hygiene Services."

|Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

[All the guidance and such]

Cost-Effective Tools
**********************************************

* CISA Cyber Hygiene Services: CISA offers several scanning and testing services to help organizations reduce their exposure to threats by taking a proactive approach to mitigating attack vectors. Types of scans and assessments include vulnerability scanning, web application scanning, phishing campaign assessments, and remote peentration testing. (https://www.cisa.gov/cyber-hygiene-services)
* ShieldsUP!: ShieldsUP is an online port scanning service that can alert the users of any ports that have been opened through their firewalls or through their NAT routers, which can be used by malicious users to take advantage of security vulnerabilities. (https://www.grc.com/shieldsup)

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************

* [links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |eges_email|.
