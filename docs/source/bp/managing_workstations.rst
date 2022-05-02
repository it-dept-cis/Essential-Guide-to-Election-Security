..
  Created by: mike garcia
  To: managing workstations

.. |bp_title| replace:: Managing Workstations

.. admonition:: Status
   :class: caution

   Soft Launch Draft

|bp_title|
----------------------------------------------

Workstation management involves configuring systems to reduce the risk of cyber attacks. Most workstations (e.g., desktop, laptops, tablets) should have capabilities limited to the job function they serve. Often, this is tied to the type of employee to which the workstation is issued. Other times, it's about the use the workstation plays in the office.

Configurations can be done manually or with automated tools.

Goals
**********************************************

#. Properly configure workstation permissions (|Maturity1| maturity)
#. Leverage CIS Benchmarks for workstation configuration (|Maturity2| maturity)

Mappings to CIS Controls and Safeguards
**********************************************

* [#.#] [title of control]
* [#.#] [title of control]

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _managing-workstations-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Limit administrative access to machines that perform administrative functions.
#. Log out machines after a short period of inactivity.
#. Employ the restrictions from the :doc:`User Management <user_management>` best practice.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Leverage the a CIS `Benchmark <https://www.cisecurity.org/cis-benchmarks/>`_ on workstation management for your operating systems.

   * Choose stricter security levels for systems with sensitive functions.
   * Consider benchmarks for desktops, laptops, mobile devices, and software on systems.
   * Use the :term:`EMS` Gateway Benchmark for machines that, through removable media, exchange data with the EMS.

Cost-Effective Tools
**********************************************

* `Applocker <https://technet.microsoft.com/en-us/library/dd759117(v=ws.11).aspx>`_: Free Microsoft® Windows tool to identify and restrict the software that is allowed to run.
* `Netwrix <https://www.netwrix.com>`_: Variety of free tools to identify information about administrative access on your systems.
* `OpenAudIT <http://www.open-audit.org/>`_: Inventory applications and software on workstation servers and network devices.

-----------------------------------------------
