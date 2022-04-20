..
  Created by: mike garcia
  To: Patching best practice largely from 2018-06-08 spotlight

.. |bp_title| replace:: Software Updates

*Best Practice:* |bp_title|
----------------------------------------------

Patching is the process of applying available software updates to an operating system, application, browser, mobile app, plugin or other type of software. While patches may bring new and useful functionality, patches are also security updates that address vulnerabilities, which could allow cyber threat actors unauthorized access to information systems or networks.

Unpatched vulnerabilities remain one of the primary infection vectors observed by the EI-ISAC and our partners. Once patches are publicly announced, information on the associated vulnerabilities they remediate is generally available to anyone, including cyber threat actors. This significantly increases the likelihood that the threat actors will attempt to exploit unpatched systems using information deduced from the patch release.

Software development companies, such as Microsoft and Adobe, regularly release bulk security patches for their products on the second Tuesday of every month, which is known as Patch Tuesday. Other companies release patches on other days of the month, quarterly, or on an ad hoc basis. In the U.S., most publicly known cybersecurity vulnerabilities are cataloged in the National Vulnerability Database (NVD) maintained by NIST. Each vulnerability in the patch is rated based on the associated level of risk, threat, and impact, along with other factors.

Successful exploitation of unpatched election infrastructure may result in data breaches, malware infections, and website defacements, among other things. Information at risk includes personally identifiable information (PII) and other voter information.

Goals
**********************************************

#.      Understand the importance of patching and how patching schedules work
#.      Know which of your systems should have timely patching and which need additional approvals

Mappings to CIS Controls and Safeguards
**********************************************

- 2.2: Ensure Authorized Software is Currently Supported
- 7.3: Perform Automated Operating System Patch Management
- 7.4: Perform Automated Application Patch Management

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

ACTION 1: Begin patching key systems on a regular timetable.

At the |Maturity1| maturity, organizations should simply begin patching their systems in a thoughtful and conssistent manner.

Every organization is different, but it's often best to start patching your operating systems first, and then move to your software applications. Network devices also need to receive software updates, but this may require a consultation with IT staff or contractors before it's agreed to patch these devices.

Devices and applications will often make patches available via a diagnostic menu or administrative console. Each device or application will be different, and this may require research. Not all systems used in elections can be patched immediately. Particularly when patching voting systems, be sure to consider your state’s or the U.S. Election Assistance Commission’s (EAC) System Certification Process and account for scheduled primary and election day system configuration freezes.

The MS-ISAC regularly disseminates _`Cybersecurity Advisories <https://www.cisecurity.org/resources/advisory/>`, which address critical patches in commercial software commonly used by government agencies and are available to all EI-ISAC members. To subscribe to Cybersecurity Advisories, EI-ISAC members should contact their account manager or complete the _`subscription form <https://learn.cisecurity.org/ms-isac-subscription>`.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

In addition to the actions at the |Maturity1| maturity, at the |Maturity2| and |Maturity3| maturities, you should ensure automated tools are being used to conduct software patching of your systems. There should also be a formal, written plan in place that references the organization's vulnerability management program, as identifying and remediating vulnerabilities goes hand-in-hand with updating software.

When creating a patch management program for your office, begin by understanding all the hardware and software assets that you are responsible for by conducting _`Asset Management <asset_managment.rst>`. Then implement a conssistent process that:
* Readily identifies patches as they become available;
* Prioritizes patches for known vulnerable systems;
* Downloads patches from authoritative sources;
* Tests and verifies patches in the operating environment; and
* Applies appropriately tested patches to vulnerable systems.

For more comprehensive recommendations and technical insight on this topic, please see the MS-ISAC’s Technical White Paper _`Timely Patching Reduces System Compromises <https://www.cisecurity.org/-/jssmedia/Project/cisecurity/cisecurity/data/media/files/uploads/2017/03/Patching-TLP-WHITE.pdf>`.

Cost-Effective Tools
**********************************************

•      [tool]: [description][(link)]
•      [tool]: [description][(link)]

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************

* Apple Auto-update - iOS
* Apple Auto-update - MacOS
* Auto-update Windows
* Auto-update MS Office on macOS
* Auto-update Android

-----------------------------------------------
