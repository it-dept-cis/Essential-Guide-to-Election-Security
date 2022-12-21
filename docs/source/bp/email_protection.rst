..
  Created by: mike garcia
  To: BP for email protection to include CIS email protection offering

.. |bp_title| replace:: Email Protection

|bp_title|
----------------------------------------------

The top cybersecurity threat to your organization is sitting in your employees’ inboxes. For all its limitations, email remains a very common mode of communication in the business environment. Email has long been a favored attack vector for cyber threat actors, using it for a wide variety of attacks, including malware and ransomware, phishing, spam, and email spoofing. According to the 2022 `Verizon Data Breach Investigations Report <https://www.verizon.com/business/resources/reports/dbir/>`_, 82% of breaches in the previous year involved the human element -- whether stolen credentials, phishing, misuse, or simple human errors.

Using email requires training and vigilance. It is a direct connection to users, which are often the weakest aspect of cybersecurity defenses. 

There are many email security trainings for end users; it's important to use one that engages and informs. It should cover:

* Basic email security
* Identifying phishing and other suspicious emails
* Social engineering
* Authentication (i.e., MFA and passphrases)
* Handling personal information and sensitive data

Deploy multi-factor authentication (MFA) on email, along with passphrases. In addition, IT administators can improve outcomes by using email protection services, which typcally enable:

* Inbound mail screening, 
* Malware and ransomware protection, 
* Phishing protection, 
* Spam filtering, 
* Email spoofing protection, 
* Traffic blocking, 
* Allowlisting of false positives, and 
* Denylisting of false negatives.

Email protection solutions vary widely in costs and complexity, so it's important to select a solution that will work well with your jurisdiction's capabilities and resources. Generally, they work as detailed in the figure below.

.. figure:: /_static/email-protection-service-flow--expanded.png
   :width: 90%
   :alt: Graphic showing the basic flow of the EI-ISAC email protection service with inbound emails being filtered through the service to identifiy potentially problematic emails.

Take email security seriously as it's so commonly used gain access to other systems. Training and email protection services are both important ways to improve your cybersecurity outcomes.


Goals
**********************************************

#. Understand the risks of using email. (|Maturity1| maturity)
#. Keep your staff propertly trained. (|Maturity1| maturity)
#. Deploy basic security measures like MFA and passphrases. (|Maturity1| maturity) 
#. Get email protection services through the EI-ISAC or commercial vendors. (|Maturity1| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _email-protection-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Provide email security training all users. Your state or county may offer a specific training, and some free ones are avaialble for governments. See :doc:`managing_staff` for more information.
#. Require MFA and passphrases wherever possible. See :doc:`user_management` for more information.
#. Deploy email protection services for all email accounts your organization uses.

   * Email protection services are provided at no cost to you by the federally-funded email protection services program. Contact |eiisac_email| for more information.
   * For commercial solutions, you may also review CIS's `Guide for Ensuring Security in Election Technology Procurements <https://www.cisecurity.org/elections>`_ for best practices in crafting proposals and other necessary documents.

.. _email-protection-maturity-two-three:

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For the |Maturity2| and |Maturity3| maturities, all of the guidance for the |Maturity1| maturity applies, but you may want to have a more sophisticated program to manage you email protection services. For instance, you may want dedicated resources to more carefully mangage advanced features like allow- and denylisting. Contact |eiisac_email| for more information.

Cost-Effective Tools
**********************************************

* `EI-ISAC Email Protection Services program brochure </_static/MS-ISAC--EPS-Email-Protection-Service--Pilot-Overview--2022-09.pdf>`_

Mapping to CIS Controls and Safeguards
**********************************************

* 9.1 Ensure only fully supported browsers and email clients are allowed to execute version of browsers and email clients provided through the vendor. (|Maturity1| maturity)
* 9.2: Use DNS filtering services on all enterprise assets to block access to known malicious domains. (|Maturity1| maturity)
* 9.3: Enforce and update network-based URL filters to limit an enterprise asset from connecting to potentially malicious or unapproved websites. Example implementations include category-based filtering, reputation-based filtering, or through the use of block lists. Enforce filters for all enterprise assets. (|Maturity1| maturity)
* 14.1: Establish and Maintain a Security Awareness Program (|Maturity1| maturity)
* 14.2: Train Workforce Members to Recognize Social Engineering Attacks (|Maturity1| maturity)
* 14.3: Train Workforce Members on Authentication Best Practices (|Maturity1| maturity)
* 14.4: Train Workforce on Data Handling Best Practices (|Maturity1| maturity)
* 14.5: Train Workforce Members on Causes of Unintentional Data Exposure (|Maturity1| maturity)
* 14.9: Conduct Role-Specific Security Awareness and Skills Training (|Maturity2| maturity)


Mapping to CIS Handbook Best Practices
****************************************

* 13, 24, 25, 57

