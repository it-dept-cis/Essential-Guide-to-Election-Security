..
  Created by: mike garcia
  To: managing infrastructure

.. |bp_title| replace:: Managing Infrastructure

|bp_title|
----------------------------------------------

Infrastructure management involves adjusting configuration settings for systems to reduce the risk of cyber attacks. Most workstations (e.g., desktop, laptops, tablets) should have capabilities limited to the job function they serve. Often, this is tied to the type of employee to which the workstation is issued, such as an admin or a poll worker. Sometimes, it's about the use the workstation plays in the office. A similar rule applies to servers and other shared infrastructure. 

.. image:: /_static/plan_implement_monitor_modify.png
  :width: 90%
  :alt: Plan Implement Monitor Modify

In general, having a few configurations you use repeatedly is better than creating custom configurations for each system you allow in your environment. You should create these configurations or get them from a trusted source and carefully track any changes to them.

Implementing these configurations can be done manually or with automated tools.

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
#. If a machine has a short period of inactivity, force a lock screen or log out.
#. Employ the restrictions from the :doc:`User Management <user_management>` best practice.
#. Work with IT staff or vendors to establish a process for configuring network infrastructure to ensure it is secure, consistent, and tracked.

.. _managing-infrastructure-maturity-two-three:

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Organizations operating at a |Maturity2| or |Maturity3| maturity should take additional actions, including:

#. Leverage the `CIS Benchmark <https://www.cisecurity.org/cis-benchmarks/>`_ on workstation management for your operating systems. This will allow for maintenance of a secure configuration process for network infrastructure.

   * Choose stricter security levels for systems with sensitive functions.
   * Consider `CIS Benchmarks <https://www.cisecurity.org/cis-benchmarks/>`_ for servers, desktops, laptops, mobile devices, and software on systems.
   * Use the :term:`EMS` Gateway `Benchmark <https://www.cisecurity.org/insights/blog/new-guidance-to-secure-election-management-system-machines>`_ for machines that, through removable media, exchange data with the EMS.
   * Uninstall or disable unnecessary services on enterprise assets and software

.. image:: /_static/infrastructure_config.png
  :width: 90%
  :alt: Infrastructue Configuration Managment Flow Diagram

Cost-Effective Tools
**********************************************

* `Applocker <https://technet.microsoft.com/en-us/library/dd759117(v=ws.11).aspx>`_: Free Microsoft® Windows tool to identify and restrict the software that is allowed to run.
* `Netwrix <https://www.netwrix.com>`_: Variety of free tools to identify information about administrative access on your systems.
* `OpenAudIT <http://www.open-audit.org/>`_: Inventory applications and software on workstation servers and network devices.
* `CIS Benchmarks <https://www.cisecurity.org/cis-benchmarks/>`_.
* EMS Gateway `Benchmark <https://www.cisecurity.org/insights/blog/new-guidance-to-secure-election-management-system-machines>`_. 

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
