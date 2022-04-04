..
  Created by: mike garcia
  On: 2022-03-17
  To: Patching best practice largely from 2018-06-08 spotlight
  Last update by: mike garcia

.. |last_update| replace:: 2022-03-17

.. include:: ../docs/source/global_directives.rst

.. |Maturity1| replace:: Reactive
.. |Maturity2| replace:: Proactive
.. |Maturity3| replace:: Adaptive

.. |contact_email| replace:: dontknowyet@cisecurity.org
.. |bp_title| replace:: Patching

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Patching is the process of applying available updates to an operating system, website, software, hardware, or plugin. In information security, patches are security updates that address identified vulnerabilities, which could allow cyber threat actors unauthorized access to information systems or networks.

Unpatched vulnerabilities remain one of the primary infection vectors observed by the EI-ISAC and our partners. Once patches are publicly announced, information on the associated vulnerabilities they remediate is generally available to anyone, including cyber threat actors. This significantly increases the likelihood that the threat actors will attempt to exploit unpatched systems using information deduced from the patch release.

Some companies, such as Microsoft and Adobe, regularly release bulk security patches for their products on the second Tuesday of every month, which is known as Patch Tuesday. Other companies release patches on other days of the month, quarterly, or on an ad hoc basis. In the U.S., most publicly known cybersecurity vulnerabilities are cataloged in the Common Vulnerabilities and Exposures (CVE) List maintained by MITRE. Each vulnerability in the patch is rated based on the associated level of risk, threat, and impact, along with other factors.

Successful exploitation of unpatched election infrastructure may result in malware infections, website defacements, or compromise the confidentiality, integrity, or availability of election-related information, which could include personally identifiable information (PII) and other voter information.

Goals
**********************************************

#.	Understand the importance of patching and how patching schedules work
#.	Know which of your systems should have timely patching and which need additional approvals

Mappings to CIS Controls and Safeguards
**********************************************

- [#.#][tab][title of control]
- [#.#][tab][title of control]

Actions
**********************************************

For |bp_title|, the necessary actions are the same for all maturity levels.

Not all systems used in elections can be patched immediately. Particularly when patching voting systems, be sure to consider your state’s or the U.S. Election Assistance Commission’s (EAC) System Certification Process and account for scheduled primary and election day system configuration freezes.

When creating a patch management program for your office, begin by understanding all the hardware and software assets that you are responsible for by conducting _`Device Asset Management <device_asset_managment.rst>`. Then implement a patch management program that:
* Readily identifies patches as they become available;
* Prioritizes patches for known vulnerable systems;
* Downloads patches from authoritative sources;
* Tests and verifies patches in the operating environment; and
* Applies appropriately tested patches to vulnerable systems.

The MS-ISAC regularly disseminates _`Cybersecurity Advisories <https://www.cisecurity.org/resources/advisory/>`, which address critical patches in commercial software commonly used by government agencies and are available to all EI-ISAC members. To subscribe to Cybersecurity Advisories, EI-ISAC members should contact their account manager or complete the _`subscription form <https://learn.cisecurity.org/ms-isac-subscription>`.

For more comprehensive recommendations and technical insight on this topic, please see the MS-ISAC’s Technical White Paper _`Timely Patching Reduces System Compromises <https://www.cisecurity.org/-/jssmedia/Project/cisecurity/cisecurity/data/media/files/uploads/2017/03/Patching-TLP-WHITE.pdf>`.

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
