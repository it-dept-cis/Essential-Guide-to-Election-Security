..
  created by: mike garcia
  to: provide a prioritized map from maturities to best practices for maturities 2 and 3

Prioritizing Best Practices for the |Maturity2| and |Maturity3| maturities
--------------------------------------------------------------------------

.. _maturity-two-and-three-maturity-baseline-priorities:

|Maturity2| and |Maturity3| Maturities
**************************************

More mature organizations should take a more sophisticated approach to prioritizing best practice implementation.

The CIS Community Defense Model
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To help organizations determine where to invest their next dollar in cybersecurity, CIS developed the :term:`Community Defense Model` (CDM). The `CDM <https://www.cisecurity.org/insights/white-papers/cis-community-defense-model-2-0>`_ was created to help answer that and other questions about the value of the :term:`CIS Controls` based on currently available threat data from industry reports. Ready more about the CIS Controls in the CIS Controls :doc:`best practice <../bp/cis_controls>`.

Using authoritative data sources like the Verizon `Data Breach Investigations Report <https://www.verizon.com/business/resources/reports/dbir/>`_, CIS identified the top attack types that enterprises should defend against. 

For CDM 2.0, the top five attack types are:

#. Malware
#. Ransomware
#. Web Application Hacking
#. Insider and Privilege Misuse
#. Targeted Intrusions 

Certain techniques are used to execute each of these types of attacks. The CDM uses the `MITRE ATT&CK framework <http://attack.mitre.org>`_ to cateogize these techniques and sub-techniques. These are mapped to mitigations, such as the Safeguards contained with the CIS Controls and the actions within this Guide's best practices, that protect against one or more sub-technique.

Using real world data, the CDM determines which Safeguards are the most efficient--the Safeguards that mitigate the most sub-techniques and thus, when implemented, are most likely to stop any given attack. 

In the table below, we map the highest efficiency Safeguards from the CIS Controls to the best practices in this Guide to establish the priority best practices. For more details on the efficiency rankings, see Figure 13 of the CDM 2.0.

This efficiency ranking drives the ordering of the best practices in this Guide, with some exceptions particular to elections. While we recommend following the prescribed order, do what's best for your environment and, most importantly, keep making progress!

.. table:: Mapping of the Most Efficient Safeguards to Priority Best Practices
   :widths: auto

   ====  =========  ===========================================================================  ===============================
   Rank  Safeguard  Safeguard Title                                                              Essential Guide Best Practice
   ====  =========  ===========================================================================  ===============================
   1     4.1        Establish and Maintain a Secure Configuration Process                        :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three>`
   2     4.7        Manage Default Accounts on Enterprise Assets and Software                    :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three>`
   3     5.3        Disable Dormant Accounts                                                     :ref:`User Management <user-management-maturity-two-three>`
   4     6.1        Establish an Access Granting Process                                         :ref:`User Management <user-management-maturity-two-three>`
   5     6.2        Establish an Access Revoking Process                                         :ref:`User Management <user-management-maturity-two-three>`
   6     5.4        Restrict Administrator Privileges to Dedicated Administrator Accounts        :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three>`
   7     18.3       Remediate Penetration Test Findings                                          :ref:`Remediate Pen Test Findings <remediate-pentest-findings-maturity-three>`
   8     18.5       Perform Periodic Internal Penetration Tests                                  :ref:`Internal Pen Testing <internal-pentest-maturity-three>`
   9     6.8        Define and Maintain Role-Based Access Control                                :ref:`User Management <user-management-maturity-two-three>`
   10    4.8        Uninstall or Disable Unnecessary Services on Enterprise Assets and Software  :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three>`
   11    3.12       Segment Data Processing and Storage Based on Sensitivity                     [Coming in 2023Q1 update]
   12    5.2        Use Unique Passwords                                                         :ref:`User Management <user-management-maturity-two-three>`
   13    6.4        Require MFA for Remote Network Access                                        :ref:`Managing Remote Connections <manage-remote-connections-maturity-two-three>`
   14    6.5        Require MFA for Administrative Access                                        :ref:`User Management <user-management-maturity-two-three>`
   15    12.8       Maintain Dedicated Computing Resources for All Administrative Work           :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three>`
   16    2.3        Address Unauthorized Software                                                :ref:`Asset Management <asset-management-maturity-two-three>`
   17    2.5        Allowlist Authorized Software                                                :ref:`Asset Management <asset-management-maturity-two-three>`
   18    4.2        Maintain a Secure Configuration Process for Network Infrastructure           :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three>`
   19    4.4        Implement and Manage a Firewall on Servers                                   :ref:`Firewalls and Port Restrictions <firewalls-ports-maturity-two-three>`
   20    6.3        Require MFA for Externally-Exposed Applications                              :ref:`User Management <user-management-maturity-two-three>`
   ====  =========  ===========================================================================  ===============================
   
The best practices in the right column are listed as priority actions in the :doc:`best practice index <../bp/bp_index>` and should be implemented first for the |Maturity2| and |Maturity3| maturities. 
