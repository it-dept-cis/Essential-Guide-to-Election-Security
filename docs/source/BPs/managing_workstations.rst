..
  Created by: mike garcia
  To: managing workstations

.. |bp_title| replace:: Managing Workstations

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Workstation management involves configuring systems to reduce the risk of cyber attacks. Most workstations (e.g., desktop, laptops, tablets) should have capabilities limited to the job function they serve. Often, this is tied to the type of employee to which the workstation is issued. Other times, it's about the use the workstation plays in the office.

Configurations can be done manually or with automated tools.

Goals
**********************************************

#.  Understand the value of restricting workstation permissions.
#.  Know where to find configuration guidance for various workstations.

Mappings to CIS Controls and Safeguards
**********************************************

- [#.#] [title of control]
- [#.#] [title of control]

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

**Actions**

#. Limit administrative access to machines that perform administrative functions.
#. Log out machines after a short period of inactivity.
#. Employ the restrictions from the :doc:`User Management <user_management.rst>` best practice.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Leverage the a CIS _`Benchmark <https://www.cisecurity.org/cis-benchmarks/>` on workstation management for your operating systems.
  * Choose stricter security levels for systems with sensitive functions.
  * Consider benchmarks for desktops, laptops, mobile devices, and software on systems.
  * Use the :term:`EMS` Gateway Benchmark for machines that, through removable media, exchange data with the EMS.

Cost-Effective Tools
**********************************************

* Applocker: Free Microsoft® Windows tool to identify and restrict the software that is allowed to run (https://technet.microsoft.com/en-us/library/dd759117(v=ws.11).aspx)
* Netwrix: Variety of free tools to identify information about administrative access on your systems (https://www.netwrix.com)
* OpenAudIT: Inventory applications and software on workstation servers and network devices (http://www.open-audit.org/)

Learn More
**********************************************
* [links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------
