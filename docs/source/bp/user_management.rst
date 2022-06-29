..
  Created by: mike garcia
  To: authN, MFA, least privilege, and related

.. |bp_title| replace:: User Management

|bp_title|
----------------------------------------------

Some of the most commonly exploited vulnerabilities are those that take place where the user meets the machine. User accounts get hijacked and are used to access resources, sometimes methodically over time, to access valuable resources or cause damage.

To reduce the risk of user account incidents, you need to implement strong protections on every user account and limit the amount of damage that may be caused by takeover of a single user account.

#. Passwords: Like it or not, passwords are a reality of online life and will be for some time to come. They are also a common vector of attack by threat actors. You can't have good user management without good password policies.
#. :term:`Multi-factor authentication` (MFA): The best way to address weaknesses in :term:`authentication` is to have the right MFA requirements in place--those that, through a variety of means, use at least two of something you know (like a password), something you have (like a cell phone), and something you are (like a fingerprint) to log in.
#. User accounts: How you manage user accounts--creating, managing, tracking, and deleting--can have a huge impact on your overall cybersecurity posture.

Goals
**********************************************

#. Implement good password practices (|Maturity1| maturity)
#. Implement :term:`MFA` wherever possible (|Maturity1| maturity)
#. Ban or limit shared or generic accounts (|Maturity1| maturity)
#. Employ least privilege, especially with administrative access, and revoke access appropriately (|Maturity1| maturity)
#. Log user activity (|Maturity1| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _user-management-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

User Recommendations
^^^^^^^^^^^^^^^^^^^^

#. Do not reuse passwords across multiple platforms, systems, or software. This includes never using the same login credentials for work and personal use.
#. Never use personal information, such as your name, children’s names, dates of birth, etc. that someone might already know or can easily obtain.
#. Use passphrases, ideally of at least four words of 5+ letters, instead of random sets of characters. If you do this, you don't need to use composition rules like upper, lower, number, and symbols. An example of a good passphrase is "blender sauté pendant chair."
#. Use a password manager, and protect access to it with MFA.

Organizational Recommendations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Remove all default accounts or change the default password on all accounts, applications, and systems.
#. Enable MFA anywhere it's offered, on all accounts, for all applications. This is especially true for anything accessed outside your environment, including social media accounts, and any access back into your environment from outside. Ensure this is true for all IT products supplied by vendors.
#. Store all passwords and passphrases using :term:`salting` and :term:`hashing` functions and **not** with reversible :term:`encryption`. Make sure your vendors do the same.
#. Set login thresholds to 10 or fewer invalid login attempts before locking the user out and increase the interval between a failed attempt and allowing the next attempt. Log and monitor all login attempts.
#. Ban or limit shared or generic accounts. In some environments, like with an e-pollbook, it might not be possible or practical to do this. Instead, rotate passwords, passcodes, and biometrics (like TouchID) when reasonable, like with each election.
#. Employ least privilege by only giving a user access to the devices, applications, and services they need to do their jobs. This limits the damage that may be caused by take over of any single account. This is particularly important for any account with administrative access to sensitive network controls or confidential materials.
#. Review individuals’ access and revoke any unnecessary or inappropriate access. Establish a plan to do this regularly, and make it part of the offboarding and job change processes to ensure that user has access to what they need and nothing else.
#. Employ user logging on your networks. You should be able to see whenever a user logs into a device or network. Maintain records of these logs.
#. Allow and encourage use of password managers.

.. _user-management-maturity-two-three:

|Maturity2| and |Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Complete all of the actions for the |Maturity1| maturity.
#. Review :term:`MS-ISAC’s <MS-ISAC>` Security Primers on Exposed Credentials and Securing Login Credentials, as well as the United States Computer Emergency Readiness Team’s (:term:`US-CERT's <US-CERT>`) Security Tip on Choosing and Protecting Passwords.
#. The :term:`EI-ISAC` regularly monitors the Internet for stolen credentials using open source datasets from various security organizations and researchers, as well as information received from trusted partners. To subscribe to this service, simply provide your IP addresses and domains to |soc_email|.
#. Use services to search for breaches of your users' email addresses and passwords.

Learn More
**********************************************

* Get more password guidance from :term:`NIST`: `SP 800-63B Section 5.1.1.2 <https://pages.nist.gov/800-63-3/sp800-63b.html#memsecretver>`_
* `Password spotlight <https://www.cisecurity.org/insights/spotlight/cybersecurity-spotlight-passwords>`_ (This spotlight has some out-of-date recommendations. Use in conjunction with the NIST guidance)
* Understand the logic behind `using passphrases <https://www.nist.gov/blogs/taking-measure/easy-ways-build-better-p5w0rd>`_.

Mapping to CIS Controls and Safeguards
**********************************************

* 4.7: Manage Default Accounts on Enterprise Assets and Software (|Maturity1| maturity)
* 5.1: Establish and Maintain an Inventory of Accounts (|Maturity1| maturity)
* 5.2: Use Unique Passwords (|Maturity1| maturity)
* 5.3: Disable Dormant Accounts (|Maturity1| maturity)
* 5.5: Establish and Maintain an Inventory of Service Accounts (|Maturity2| maturity)
* 5.6: Centralize Account Management (|Maturity2| maturity)
* 6.1: Establish an Access Granting Process (|Maturity1| maturity)
* 6.2: Establish an Access Revoking Process (|Maturity1| maturity)
* 6.3: Require MFA for Externally-Exposed Applications (|Maturity1| maturity)
* 6.4: Require MFA for Remote Network Access (|Maturity1| maturity)
* 6.5: Require MFA for Administrative Access (|Maturity1| maturity)
* 6.6: Establish and Maintain an Inventory of Authentication and Authorization Systems (|Maturity2| maturity)
* 6.7: Centralize Access Control (|Maturity2| maturity)
* 6.8: Define and Maintain Role-Based Access Control (|Maturity2| maturity)

Mapping to CIS Handbook Best Practices
****************************************

* 24, 25, 26, 47, 49, 50, 51, 52, 66, 77, 78, 81
