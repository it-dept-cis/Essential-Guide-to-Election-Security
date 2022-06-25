..
  created by: mike garcia
  to: provide a map from maturities to best practices. this is a shortcut for all maturities. individual pointers should exist in each maturity and this is a summary of them

Maturity Alignment to Best Practices
----------------------------------------------

This section provides baseline goals for each maturity and maps these to best practices. Each best practice is placed in one of three groups. We recommend you implement based on those groupings, but adjust as it makes sense for your organization.

.. _maturity-mapping-to-bp-maturity-one-description:

|Maturity1| Maturity
***************************************

If you are at the |Maturity1| maturity, your first goal should be to commit to incrementally improving your maturity. This is about setting simple goals: complete one simple task a week, implement one best practice a month, and set aside a minimum set of resources dedicated to cybersecurity every quarter. Whatever helps you make progress.

.. _maturity-one-maturity-baseline-priorities:

|Maturity1| Maturity Baseline Priorities
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The following is the list of priority actions at the |Maturity1| maturity. If you are at the |Maturity1| maturity, we recommend starting with these to establish a baseline of cyber hygiene.

**Actions**

1. Download and complete the :doc:`worksheets <../appendices/worksheets>` for |Maturity1| maturity baseline.

Together, these fulfill all of the |Maturity1| baseline priorities:

+----------------------+-----------------------------------------------------------------------+------------------+
| Worksheet            | Best Practice                                                         | Actions Covered  |
+======================+=======================================================================+==================+
| Hardware Inventory   |                                                                       |                  |
| Software Inventory   |                                                                       |                  |
| Data Inventory       | :ref:`Asset Management <asset-management-maturity-one>`               | #1               |
| Service Provider     |                                                                       |                  |
| Inventory            |                                                                       |                  |
| Account Inventory    |                                                                       |                  |
+----------------------+-----------------------------------------------------------------------+------------------+
| Asset Protection     | :ref:`Encrypt Data At Rest <encrypt-data-at-rest-maturity-one>` &     | All              |
|                      | :ref:`Managing Infrastructure <managing-infrastructure-maturity-one>` | #1 and #2        |
+----------------------+-----------------------------------------------------------------------+------------------+
| Account Security     | :ref:`User Management <user-management-maturity-one>`                 | All User         |
|                      |                                                                       | Recommendations  |
+----------------------+-----------------------------------------------------------------------+------------------+
| Backup & Recovery    | :ref:`Backups <backups-maturity-one>`                                 | All              |
+----------------------+-----------------------------------------------------------------------+------------------+
| Incident Response    | :ref:`Incident Response <incident-response-maturity-one>`             | All              |
+----------------------+-----------------------------------------------------------------------+------------------+
| Cyber Education      | :ref:`Building and Managing Staff <managing-staff-maturity-one>`      | All              |
+----------------------+-----------------------------------------------------------------------+------------------+

While the needed effort can vary greatly depending on the size of your office and number of assets (computers, software, etc.), each exercise is built to take no more than four hours the first time around and as little as 15 minutes each subsequent time. A suggestions: set aside time to do one a week until you've got them all done; then they're easy to repeat.

.. _maturity-one-maturity-election-priorities:

|Maturity1| Maturity Election Priorities
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In addition to the above, you should be implementing some measures of particular importance to the election community:

1.  Join the :doc:`EI-ISAC <../bp/join_ei_isac>`.
#.  :doc:`Protect your website <../bp/websites>` with simple and free tools.
#.  Implement an :doc:`endpoint protection <../bp/endpoint_protection>` program through a commercial provider or for free through the EI-ISAC.
#.  Implement the :doc:`malicious domain blocking and reporting <../bp/mdbr>` tool for free through the EI-ISAC.
#.  A :doc:`removable media sanitization program <../bp/removable_media>`.
#.  Establish a baseline incident response and recovery program (best practice coming in phase 2).

..
    #. Become a member of the `EI-ISAC’s Peer Support Tool <url>`_ so you can ask questions and find practical guidance from election officials facing the same concerns as you.

.. _maturity-two-and-three-maturity-baseline-priorities:

|Maturity2| and |Maturity3| Maturities
**************************************

No one wants to suffer a cybersecurity incident. The intent to protect networks is universal, but resource limitations leave many organizations facing perhaps the most difficult question in all of cybersecurity: What do I do next?

The CIS Community Defense Model
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To help answer question of where cybersecurity practioners should invest their next dollar, CIS developed the Community Defense Model (:term:`CDM`). The `CDM <https://www.cisecurity.org/insights/white-papers/cis-community-defense-model-2-0>`_ was created to help answer that and other questions about the value of the :term:`CIS Controls` based on currently available threat data from industry reports. Ready more about the CIS Controls in the CIS Controls :doc:`best practice <../bp/cis_controls>`.

Using authoritative data sources like the Verizon `Data Breach Investigations Report <https://www.verizon.com/business/resources/reports/dbir/>`_, CIS identified the top attack types that enterprises should defend against. 

The top five attack types are:

#. Malware
#. Ransomware
#. Web Application Hacking
#. Insider and Privilege Misuse
#. Targeted Intrusions 

Certain techniques are used to execute each of these types of attacks. The CDM uses the MITRE ATT&CK framework to cateogize these techniques and sub-techniques. These are mapped to mitigations, such as the Safeguards contained with the CIS Controls and the actions within this Guide's best practices, that protect against one or more sub-technique.

The goal of the CDM is to determine with mitigations are most effective at thwarting attacks. Using real world data, the CDM determines which Safeguards are the most efficient--the Safeguards that mitigate the most sub-techniques and thus, when implemented, are most likely to stop any given attack. 

In the table below, we map the highest efficiency Safeguards from the CIS Controls to the best practices in this Guide to establish the priority best practices. For more details on the efficiency rankings, see Figure 13 of the CDM 2.0.

.. table:: CIS Most Efficient Safeguard Mapping to Priority Best Practices
   :widths: auto

   ====  =========  ===========================================================================  ===============================
   Rank  Safeguard  Safeguard Title                                                              Essential Guide Best Practice
   ====  =========  ===========================================================================  ===============================
   1     4.1        Establish and Maintain a Secure Configuration Process                        :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three`
   2     4.7        Manage Default Accounts on Enterprise Assets and Software                    :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three`
   3     5.3        Disable Dormant Accounts                                                     :ref:`User Management <user-management-maturity-two-three>`
   4     6.1        Establish an Access Granting Process                                         :ref:`User Management <user-management-maturity-two-three>`
   5     6.2        Establish an Access Revoking Process                                         :ref:`User Management <user-management-maturity-two-three>`
   6     5.4        Restrict Administrator Privileges to Dedicated Administrator Accounts        :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three`
   7     18.3       Remediate Penetration Test Findings                                          [Coming in 2022Q3 update]
   8     18.5       Perform Periodic Internal Penetration Tests                                  [Coming in 2022Q3 update]
   9     6.8        Define and Maintain Role-Based Access Control                                :ref:`User Management <user-management-maturity-two-three>`
   10    4.8        Uninstall or Disable Unnecessary Services on Enterprise Assets and Software  :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three`
   11    3.12       Segment Data Processing and Storage Based on Sensitivity                     [Coming in 2022Q3 update]
   12    5.2        Use Unique Passwords                                                         :ref:`User Management <user-management-maturity-two-three>`
   13    6.4        Require MFA for Remote Network Access                                        :ref:`Managing Remote Connections <managing-remote-connections-maturity-two-three>`
   14    6.5        Require MFA for Administrative Access                                        :ref:`User Management <user-management-maturity-two-three>`
   15    12.8       Maintain Dedicated Computing Resources for All Administrative Work           :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three`
   16    2.3        Address Unauthorized Software                                                :ref:`Asset Management <asset-management-maturity-two-three>`
   17    2.5        Allowlist Authorized Software                                                :ref:`Asset Management <asset-management-maturity-two-three>`
   18    4.2        Maintain a Secure Configuration Process for Network Infrastructure           :ref:`Managing Infrastructure <managing-infrastructure-maturity-two-three`
   19    4.4        Implement and Manage a Firewall on Servers                                   :ref:`Firewalls and Port Restrictions <_firewalls-ports-maturity-two-three>`
   20    6.3        Require MFA for Externally-Exposed Applications                              :ref:`User Management <user-management-maturity-two-three>`
   ====  =========  ===========================================================================  ===============================
   
The best practices in the right column are listed as priority actions in the best practice index and should be implemented first of the |Maturity2| and |Maturity3| maturities. 

------------------
