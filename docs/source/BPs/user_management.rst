..
  Created by: mike garcia
  To: authN, MFA, least privilege, and related

.. |bp_title| replace:: User Management

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Some of the most commonly exploited vulnerabilities are those that take place where the user meets the machine. User accounts get hijacked and are used to access resources, sometimes methodically over time, to access valuable resources or cause damage.

To reduce this risk, you both need strong protections on every user account and limitations on the amount of damage that can be done when a single user account going bad.

Goals
**********************************************

#.  Understanding good password practices, like requiring passphrases and salting and hashing them
#.  Knowing when to require multi-factor authentication (:term:MFA)
#.  Understanding when to ban or limit shared or generic accounts
#.  Knowing about least privilege, especially with administrative access, and revoking access
#.  Understanding user activity logging

Mappings to CIS Controls and Safeguards
**********************************************

- [#.#] [title of control]
- [#.#] [title of control]

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Passwords
%%%%%%%%%%%%%%%%%%%%%%

**User Recommendations**
* Do not reuse passwords across multiple platforms, systems, or software. This includes never using the same login credentials for work and personal use.
* Never use personal information, such as your name, children’s names, dates of birth, etc. that someone might already know or can easily obtain.
* Use passphrases, ideally of at least four words of 5+ letters, instead of random sets of characters. If you do this, you don't need to use composition rules like upper, lower, number, and symbols

**Organizational Recommendations**
* Remove all default accounts or change the default password on all accounts, applications, and systems.
* Store all passwords and passphrases using salting and hashing functions and **not** with reversible encryption
* Set login thresholds to 10 or fewer invalid login attempts and require at least 15 minutes between account lockout. Log and monitor all login attempts.

Multi-factor authentication
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

* Enable MFA anywhere it's offered, on all accounts, for all applications. This is especially true for anything accessed offsite or from offsite, including social media accounts. Ensure this is true for all IT products supplied by vendors.

*  Understanding when to ban or limit shared or generic accounts

#.  Knowing about least privilege, especially with administrative access, and revoking access
#.  Understanding user activity logging


|Maturity2| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

MS-ISAC’s Security Primers on Exposed Credentials and Securing Login Credentials, as well as the United States Computer Emergency Readiness Team’s (US-CERT) Security Tip on Choosing and Protecting Passwords.
The EI-ISAC regularly monitors the Internet for stolen credentials using open source datasets from various security organizations and researchers, as well as information received from trusted partners. To subscribe to this service, simply provide your IP addresses and domains to soc@cisecurity.org.


|Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

[All the guidance and such]

Cost-Effective Tools
**********************************************

* [tool]: [description][(link)]
* [tool]: [description][(link)]

Learn More
**********************************************
* 800-63B Section 5.1.1.2
* _`Password spotlight <https://www.cisecurity.org/insights/spotlight/cybersecurity-spotlight-passwords>` (note this spotlight has some out-of-date recommendations)

-----------------------------------------------
