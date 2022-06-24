..
  Created by: mike garcia
  To: managing infrastructure

.. |bp_title| replace:: Managing Infrastructure

.. admonition:: Status
   :class: caution

   Soft Launch Draft

|bp_title|
----------------------------------------------

Infrastructure management involves configuring systems to reduce the risk of cyber attacks. Most workstations (e.g., desktop, laptops, tablets) should have capabilities limited to the job function they serve. Often, this is tied to the type of employee to which the workstation is issued. Other times, it's about the use the workstation plays in the office.

Servers and other such infrastructure should have secure configurations that are consistent and have changes carefully tracked. 

Configurations can be done manually or with automated tools.

Goals
**********************************************

#. Properly configure workstation permissions (|Maturity1| maturity)
#. Leverage CIS Benchmarks for workstation and infrastructure configuration (|Maturity2| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _managing-infrastructure-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Limit administrative access to machines that perform administrative functions.
#. Log out machines after a short period of inactivity.
#. Employ the restrictions from the :doc:`User Management <user_management>` best practice.
#. Establish a process for configuring network infrastructre to ensure it is secure, consistent, and tracked.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Leverage the a CIS `Benchmark <https://www.cisecurity.org/cis-benchmarks/>`_ on workstation management for your operating systems. This will allow for maintenance of a secure configuration process for network infrasturcture.

   * Choose stricter security levels for systems with sensitive functions.
   * Consider benchmarks for servers, desktops, laptops, mobile devices, and software on systems.
   * Use the :term:`EMS` Gateway Benchmark for machines that, through removable media, exchange data with the EMS.
   * Uninstall or disable unnecessary services on enterprise assets and software

Cost-Effective Tools
**********************************************

* `Applocker <https://technet.microsoft.com/en-us/library/dd759117(v=ws.11).aspx>`_: Free Microsoft® Windows tool to identify and restrict the software that is allowed to run.
* `Netwrix <https://www.netwrix.com>`_: Variety of free tools to identify information about administrative access on your systems.
* `OpenAudIT <http://www.open-audit.org/>`_: Inventory applications and software on workstation servers and network devices.

Mapping to CIS Controls and Safeguards
**********************************************

* 4.3: Configure Automatic Session Locking on Enterprise Assets (|Maturity1| maturity)
* 5.4: Restrict Administrator Privileges to Dedicated Administrator Accounts (|Maturity1| maturity)
* 4.2: Maintain a Secure Configuration Process for Network Infrastructure (|Maturity1| maturity)
* 12.8: Establish and Maintain Dedicated Computing Resources for All Administrative Work (|Maturity1| maturity)
* 4.8: Uninstall or Disable Unnecessary Services on Enterprise Assets and Software (|Maturity2| maturity)

Mapping to CIS Handbook Best Practices
****************************************

* 23, 27, 65, 68, 88

-----------------------------------------------
