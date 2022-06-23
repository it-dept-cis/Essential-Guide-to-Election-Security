..
  Created by: mike garcia
  To: Incident Response

.. |bp_title| replace:: Incident Response

.. admonition:: Status
   :class: caution

   Soft Launch Draft

|bp_title|
----------------------------------------------

Some of the most commonly exploited vulnerabilities are those that take place where the user meets the machine. User accounts get hijacked and are used to access resources, sometimes methodically over time, to access valuable resources or cause damage.

To reduce this risk, you both need strong protections on every user account and limitations on the amount of damage that can be done when a single user account goes bad.

#. Passwords: Like it or not, passwords are a reality of online life and will be for some time to come. They are also common vector of attack by threat actors. You can't have good user management without good password policies.
#. Multi-factor authentication (:term:`MFA`): The best way to address weaknesses in :term:`authentication` is to have the right MFA requirements in place.
#. User accounts: How you manage user accounts--creating, managing, tracking, and deleting--can have a huge impact on your overall cybersecurity posture.

Goals
**********************************************

#. Implement good password practices, like requiring passphrases and salting and hashing them (|Maturity1| maturity)
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
#. Use passphrases, ideally of at least four words of 5+ letters, instead of random sets of characters. If you do this, you don't need to use composition rules like upper, lower, number, and symbols.
#. Use a password manager, and protect access to it with MFA.

Organizational Recommendations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Remove all default accounts or change the default password on all accounts, applications, and systems.
#. Enable MFA anywhere it's offered, on all accounts, for all applications. This is especially true for anything accessed offsite or from offsite, including social media accounts. Ensure this is true for all IT products supplied by vendors.
#. Store all passwords and passphrases using salting and hashing functions and **not** with reversible encryption. Make sure your vendors do the same.
#. Set login thresholds to 10 or fewer invalid login attempts and require at least 15 minutes between account lockout. Log and monitor all login attempts.
#. Ban or limit shared or generic accounts. In some environments, like with an e-pollbook, it might not be possible or practical to do this. Instead, rotate passwords, passcodes, and biometrics (like TouchID) when reasonable, like with each election.
#. Employ least privilege by only giving a user access to the devices, applications, and services they need to do their jobs. This limits the damage any single account can do when taken over. This is why it's critical to do this for any account with administrative access
#. Revoke access. Establish a plan to review access regularly, and make it part of the offboarding and job change processes to ensure that user has access to what they need and nothing else.
#. Employ user logging on your networks. You should be able to tell when, and maintain a record of, a user logs into a device or network.
#. Allow and encourage use of password managers.


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

* [#.#] [title of control]
* [#.#] [title of control]

Mapping to CIS Handbook Best Practices
****************************************

* a

-----------------------------------------------
