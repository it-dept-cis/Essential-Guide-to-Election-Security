..
  Created by: mike garcia
  To: Patching best practice largely from 2018-06-08 spotlight

.. |bp_title| replace:: Patching and Vulnerability Management

|bp_title|
----------------------------------------------

:term:`Patching` is the process of applying available software updates to an operating system, application, browser, mobile app, plugin or other type of software. While patches may bring new and useful functionality, patches are also security updates that address known vulnerabilities that could allow cyber threat actors unauthorized access to information systems or networks. While there are some differences, for the purposes of this guide, patching and vulnerability management are synonymous.

Unpatched vulnerabilities remain one of the primary infection vectors observed by the :term:`EI-ISAC` and our partners. Once patches are publicly announced, information on the associated vulnerabilities they remediate is generally available to anyone, including cyber threat actors. This significantly increases the likelihood that the threat actors will attempt to exploit unpatched systems using information deduced from the patch release.

Software development companies, such as Microsoft and Adobe, regularly release bulk security patches for their products on the second Tuesday of every month, which is known as Patch Tuesday. Other companies release patches on other days of the month, quarterly, or on an ad hoc basis. In the U.S., most publicly known cybersecurity vulnerabilities are cataloged in the `National Vulnerability Database <https://nvd.nist.gov>`_ (:term:`NVD`) maintained by :term:`NIST`. Each vulnerability in the patch is rated based on the associated level of risk, threat, and impact, along with other factors. The NVD `frequently asked questions <https://nvd.nist.gov/general/FAQ-Sections/General-FAQs>`_ provide a wealth of information on the NVD.

Successful exploitation of unpatched election infrastructure may result in data breaches, malware infections, and website defacements, among other things. Information at risk includes personally identifiable information (:term:`PII`) and other voter information.

The :term:`MS-ISAC` regularly disseminates `Cybersecurity Advisories <https://www.cisecurity.org/resources/advisory/>`_, which address critical patches in commercial software commonly used by government agencies and are available to all :term:`EI-ISAC` members. To subscribe to Cybersecurity Advisories, :term:`EI-ISAC` members should contact their account manager or complete the `subscription form <https://learn.cisecurity.org/ms-isac-subscription>`_.

Goals
**********************************************

#. Understand the importance of patching (|Maturity1| maturity)
#. Establish a patching schedules (|Maturity1| maturity)
#. Establish and execute on a policy for systems that need additional approvals prior to patching (|Maturity1| maturity)
#. Establish a formal patch management plan leveraging automated tools and aligned with your asset management plan (|Maturity2| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

At the |Maturity1| maturity, organizations should simply begin patching their systems in a thoughtful and consistent manner.

Devices and applications will often make patches available via a diagnostic menu or administrative console. Each device or application will be different, and this may require research. Not all systems used in elections can be patched immediately. Particularly when patching voting systems, be sure to consider your state’s or the U.S. Election Assistance Commission’s (:term:`EAC`) System Certification Process and account for scheduled primary and election day system configuration freezes.

#. Verify that all software used in the office is supported by an active development company. If not, update or replace the software. Only download patches from authoritative sources.
#. Patch all operating systems on a regular timetable.

   * Every organization is different, but it's often best to start patching your operating systems first, and then move to your software applications. Systems should be set to update by automatically. Network devices also need to receive software updates, but this may require a consultation with IT staff or contractors before it's agreed to patch these devices.

#. Patch all software applications on a regular timetable.
#. Where complex or mission critical systems are used, test and verify patches before patching production systems. 

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Use automated tools to conduct software patching of your systems.
#. Establish a formal, written plan in place that references the organization's vulnerability management program, as identifying and remediating vulnerabilities goes hand-in-hand with updating software.

   * When creating a patch management program for your office, begin by understanding all the hardware and software assets that you are responsible for by conducting :doc:`Asset Management <asset_management>`. Then implement a conssistent process that:

     * Readily identifies patches as they become available;
     * Prioritizes patches for known vulnerable systems;
     * Downloads patches from authoritative sources;
     * Tests and verifies patches in the operating environment; and
     * Applies appropriately tested patches to vulnerable systems.

For more comprehensive recommendations and technical insight on this topic, please see the MS-ISAC’s Technical White Paper `Timely Patching Reduces System Compromises <https://www.cisecurity.org/-/jssmedia/Project/cisecurity/cisecurity/data/media/files/uploads/2017/03/Patching-TLP-WHITE.pdf>`_.

Cost-Effective Tools
**********************************************

* `Itarian <https://www.itarian.com>`_: Patch management solution for Windows
* `Opsi <https://www.opsi.org>`_: A more complicated solution that can help to manage both Windows and Linux platforms
* `OpenVAS <https://www.openvas.org>`_: Free, open-source framework for vulnerability scanning and management

Learn More
**********************************************

* The MS-ISAC’s Technical White Paper `Timely Patching Reduces System Compromises <https://www.cisecurity.org/-/jssmedia/Project/cisecurity/cisecurity/data/media/files/uploads/2017/03/Patching-TLP-WHITE.pdf>`_
* `Apple Auto-update - iOS <https://support.apple.com/en-us/HT202180>`_
* `Apple Auto-update - MacOS <https://support.apple.com/en-us/HT201541>`_
* `Auto-update Windows <https://support.microsoft.com/en-us/windows/keep-your-pc-up-to-date-de79813c-7919-5fed-080f-0871c7bd9bde>`_
* `Auto-update MS Office on macOS <https://support.microsoft.com/en-us/office/update-office-for-mac-automatically-bfd1e497-c24d-4754-92ab-910a4074d7c1?ui=en-us&rs=en-us&ad=us>`_
* `Auto-update Android <https://support.google.com/googleplay/answer/113412>`_

Mapping to CIS Controls and Safeguards
**********************************************

* 2.2: Ensure Authorized Software is Currently Supported
* 7.3: Perform Automated Operating System Patch Management
* 7.4: Perform Automated Application Patch Management

Mapping to CIS Handbook Best Practices
****************************************

* 43, 44, 76
