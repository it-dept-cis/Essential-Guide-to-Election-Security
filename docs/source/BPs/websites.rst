..
  Created by: mike garcia
  To: websites, including .gov, https, dos, typosquatting, defacements

.. |bp_title| replace:: Website Security Basics

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

An election office's website is often the first and most important source of information for voter, the media, and other interested parties. It is extremely important to have a secure website that prevents attacks, looks official, and provides critical information.

This best practice covers five important topics about websites:

1. The .gov top-level domain
Top-level domains are important to understand both from a cybersecurity perspective and to know how constituents will engage with and access your web presence. The “.gov” domain suffix is restricted to verified U.S. government entities, which helps ensure legitimacy for visitors browsing U.S. government websites. Additionally, “.gov” domain owners are required to maintain a higher level of security and the federal government has implemented several cybersecurity controls in the underlying infrastructure.

As .gov domains are carefully controlled, once you have one you can communicate to your constituents that they should only trust a .gov for official information.

2. Securing a site with HTTPS*
Hyper Text Transfer Protocol Secure (HTTPS) is an internet communication protocol used to encrypt and securely transmit information between a user’s web browser and the website they are connected to. HTTPS accomplishes this through the use of a Secure Sockets Layer (SSL) certificate, which establishes an encrypted connection. The certificate also helps authenticate that the website and the user are who they say they are when communicating.

HTTPS is the norm across the internet. Major web browsers mark websites that do not use HTTPS as not secure and often require users to make take additional steps to visit the site. Even if the site doesn't contain malicious content, this can dissuade people from trusting your official site.

3. About denial of service attacks
A denial of service attack (DoS) seeks to disrupt the availability of a system or service. Typically, these attacks target webservers in order to overwhelm the webserver’s internet connection or its ability to respond to user requests. If the attacker can send more requests than permitted by the system, the webserver or internet connection will be too busy to respond to additional requests, resulting in a “denial of service” to legitimate users. Attackers may use multiple source computers in a distributed denial of service (DDoS) attack. Of note, computers participating in a DDoS attack may be infected with malware that conducts the attack, which means they are also victims of malicious activity.

4. Recognizing typosquatting
Typosquatting attempts to take advantage of errors users might when URLs are typed directly into the address bar. Similarly, malicious actors may seek to trick users taking a quick glance at a URL into opening a visually similar, yet malicious link.

5. Understanding website defacements
Website defacements are the unauthorized modification of web pages, including the addition, removal, or alteration of existing content. Websites that are unpatched or misconfigured are easily susceptible to simple probing tools used by these actors, which can lead to unauthorized access to websites.

While in most cases they seem to be simply a nuisance, website defacements pose a potential public relations concern for election offices, and could promote disinformation, including the alteration of time and dates for open voting events or unofficial results. These changes may be subtle and thus difficult to detect.

Goals
**********************************************

#.	Understand the .gov top-level domain and why it's important
#.	Know why HTTPS matters and how to ensure your site is protected with it
#.  Understand denial of service attacks and how to prevent them
#.  Understand typosquatting and what to do about it
#.  Know about website defacements and how to prevent them

Mappings to CIS Controls and Safeguards
**********************************************

There are no relevant CIS Controls.

Actions
**********************************************

For |bp_title|, the necessary actions are the same for all maturity levels.

#. Visit https://dotgov.gov to sign up for and manage a .gov domain.
  * Effectively managing a website can be difficult, but the good news is that you can mitigate many of the risks with one simple step: getting a .gov domain. A .gov domain automatically provides HTTPS and reduces the likelihood of your constituents confusing other websites for yours.
#. Stop DOS attacks by using no-cost tools
  * Tool include those from from _`Cloudflare <https://www.cloudflare.com/athenian/>` and _`Google <https://projectshield.withgoogle.com/landing>` will mitigate instances of these attacks.
  * Learn more through the EI-ISAC's _`Guide to DDoS Attacks <https://www.cisecurity.org/insights/white-papers/technical-white-paper-guide-to-ddos-attacks>`.
#. Reduce the risk of typosquatting by
  * Communicating that your .gov site is the only official site
  * Register or purchase variations of your domain, such as your domain but with .com, .org, and .net addresses and common typos that might occur.
#. Manage website defacements by
  * Developing a plan to defend against and recover from website defacements
    * Consider temporarily pulling down the site to prevent any further misrepresentation
    * Have a recovery plan created on how to alert readers about the targeted website.
    * Have offline backups established that can be quickly deployed in place of a compromised website.
  * Maintain up-to-date software
  * Enroll in CISA's _`CyHy program <https://www.cisa.gov/cyber-hygiene-web-application-scanning>` or the EI-ISAC’s _`Vulnerability Assessment <https://www.cisecurity.org/ei-isac/ei-isac-services>` to receive notifications on outdated software

Cost-Effective Tools
**********************************************

•	DotGov.gov: The government portal to obtain and manage a .gov domain  https://dotgov.gov
•	_`CyHy program <https://www.cisa.gov/cyber-hygiene-web-application-scanning>`
• _`Cloudflare <https://www.cloudflare.com/athenian/>`
• _`Google <https://projectshield.withgoogle.com/landing>`

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************
•	_`Election Security Spotlight – Typosquatting <https://www.cisecurity.org/insights/spotlight/ei-isac-cybersecurity-spotlight-typosquatting>`
•	_`Defending the 2018 Midterm Elections from Foreign Adversaries <https://media.defcon.org/DEF%20CON%2026/DEF%20CON%2026%20presentations/DEFCON-26-Joshua-Franklin-and-Kevin-Franklin-Defending-the-2018-Midterm-Elections.pdf>`

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |eges_email|.

This page last updated on |last_update|.
