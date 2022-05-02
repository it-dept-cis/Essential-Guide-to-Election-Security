..
  Created by: mike garcia
  To: cover firewall protections and port restrictions

.. |bp_title| replace:: Firewalls and Port Restrictions

.. admonition:: Status
   :class: caution

   Soft Launch Draft

|bp_title|
----------------------------------------------

Firewalls are an important part of cyber defense. You can set policies to manage firewalls to prevent unwanted behavior and reduce the risk of successful attack. On the other hand, a poorly protected firewall or bad configuration decisions can give threat actors an opportunity to gain access to private assets and resources.

Attackers search for vulnerable default settings, gaps or inconsistencies in firewall rule sets, routers, and switches and use those holes to penetrate defenses. They exploit flaws in these devices to gain access to networks, redirect traffic on a network, and intercept data while in transmission.

All firewalls, no matter how simple or small of a network, need to have their configurations managed. To properly manage network firewalls, you need to establish rules and policies, tracking changes, and monitoring compliance logs. You should also implement and manage firewalls on end user devices.

Goals
**********************************************

#. Enable network scanning to look for port vulnerabilities (|Maturity1| maturity)
#. Enable firewall management on networks (|Maturity1| maturity)
#. Enable firewall management on end-user devices (|Maturity1| maturity)

Mappings to CIS Controls and Safeguards
**********************************************

* [#.#] [title of control]
* [#.#] [title of control]

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Manage firewalls on all servers and end-user devices.

#. Use free tools and services to conduct scans of your publicly-facing assets. This should include your website and any online portals you are responsible for that are used for elections purposes. Sign up for free vulnerability scanning by contacting CISA at |CISA_vuln_email| with subject line "Requesting Cyber Hygiene Services."
#. Change default passwords for all applications, operating systems, routers, firewalls, wireless access points, printer/scanners, and other devices when adding them to the network.
#. Block all access by default, then allow-list traffic you want on the network.
#. Update firewall software automatically or on a set schedule. Stick to that schedule.
#. Limit administrative access to the firewalls to as few individuals as possible.
#. Review firewall rules on a set schedule. Stick to that schedule.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Take more advance measures to manage firewalls.

#. Implement a `CIS Benchmark`_ for firewall management.

Cost-Effective Tools
**********************************************

* Free vulnerability scanning from CISA (contact |CISA_vuln_email| with subject line "Requesting Cyber Hygiene Services")
* `CIS Benchmark`_ for firewall management

-----------------------------------------------

.. _CIS Benchmark: https://www.cisecurity.org/cis-benchmarks/
