..
  Created by: mike garcia
  On: 2022-02-27
  To: Backups. Derived largely from dec 2018 spotlight
  Last update by: mike garcia

.. |bp_title| replace:: Backups

|bp_title|
----------------------------------------------

Backups are necessary due to the constant threat of modification or erasure of data due to accidental deletions, :term:`malware` (including :term:`ransomware`), natural disasters, or other events. Good backup practices are especially important during critical points of operational cycles, like the beginning of early voting.

Backups play a crucial role in expediting the recovery from malicious cyber activity, allowing the restoration of a system to a reliable state that is free of malware and retains the original data. Rebuilding or re-imaging an infected system from a known good backup or fresh operating system installation is a common best practice in incident response. For instance, if an elections network is compromised due to malware, restoring systems from a clean, uncompromised backup will allow the system to be quickly remediated and put back into production without having to wait to identify remove all possible malicious files.

Backup programs should developed based on six characteristics:

#. **Data Classification:** Knowing what you want to backup will help you determine what and how frequently that data should be backed up. For instance, data vital to election operations, such as voter registration information, would be considered a high priority, and the risk management process may justify the use of nightly full backups. Retention requirements can play a role in classification.
#. **Frequency:** Consider how much data loss would be acceptable in the event of a catastrophic failure. The amount of data that would be acceptable to lose (e.g., 24 hours’ worth) should then be used to determine how often data should be backed up.
#. **Encrypted:** Backups should be encrypted. Having the backup encrypted will safeguard it if an unauthorized individual tries to access it.
#. **Offline:** Backups must be stored offline to reduce the risk of malware infecting the copies. Some malware, such as ransomware, will specifically look for backups that are available on the network to hinder the recovery process.
#. **Offsite:** Backups should be stored offsite to ensure recovery is possible in the event of disasters, such as fire or flooding. Offsite backups could be physical copies or cloud-based. The backup location is vital to the recovery process and must be a place where the backups will be secure but quickly accessible.
#. **Tested:** Testing the backup’s integrity and the ability to successfully restore a system from the backup is essential to a successful restoration. This ensures that, if needed, the backups will be able to restore what has been corrupted or destroyed. Too often backups are untested and can't actually be restored in times of crisis.

Goals
**********************************************

#. Create a procedure for backups
#. Implement automated backups
#. Protect backups
#. Test your recovery plan

Mappings to CIS Controls and Safeguards
**********************************************

* 11.1: Establish and maintain a data recovery process (|Maturity1| maturity)
* 11.2: Perform automated backups of in-scope enterprise assets (|Maturity1| maturity)
* 11.3: Protect recovery data (|Maturity1| maturity)
* 11.4: Establish and maintain an isolated instance of recovery data (|Maturity1| maturity)
* 11.5: Test backup recovery (|Maturity2| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

Creating a data inventory for a reactive maturity organization should include, at a minimum:

* voter registration information
* ballot definitions
* election equipment security processes

.. _backups-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Perform a data inventory to understand the most important data residing within your network.
#. Ensure data critical to the operation of your state organization or local jurisdiction is backed up and stored offsite.

There are many automated methods for creating backups. Most solutions are encrypted and can be set to the desired frequency. But many are only either offline or offsite, whereas both are necessary to have a complete backup program. Offline backups help protect from ransomware, while offsite backups help protect from local disasters.

Simple built-in backup tools like Apple's Time Machine and Microsoft's Backup and Restore work well for offline backups if they are not kept connected to a network or machine. If you wish to use tools like this, be sure to have a plan to connect them on a prescribed schedule and then promptly remove, isolate, and securely store them. Unless you move them to other locations, they are not good solutions for offsite backups.

Either implement a tool that provides both offline and offsite backup capabilities or implement multiple tools. Some are described below within Cost-Effective Tools.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Complex systems require complex solutions, and this can apply to backups as well. Solutions should conform to your data management plan.

Backups should be tested at least once a quarter and whenever processes or technologies are changed to ensure they can rapidly restore operations if needed.

Cost-Effective Tools
**********************************************

* `Apple Time Machine <https://support.apple.com/en-us/HT201250>`_: Time Machine is the backup mechanism of macOS, the desktop operating system developed by Apple. The software is designed to work with both local storage devices and network-attached disks and is most commonly used with external disk drives connected using either USB or Thunderbolt.
* `Amanda Network Backup <http://www.amanda.org>`_: AMANDA, the Advanced Maryland Automatic Network Disk Archiver, is a backup solution that allows the IT administrator to set up a single master backup server to back up multiple hosts over network to tape drives/changers or disks or optical media. Amanda uses native utilities and formats (e.g. dump and/or GNU tar) and can back up a large number of servers and workstations running multiple versions of Linux or Unix. Amanda uses a native Windows client to back up Microsoft Windows desktops and servers.
* `Bacula <http://blog.bacula.org/doku.php>`_: Bacula is a set of Open Source computer programs that permit you (or the system administrator) to manage backup, recovery, and verification of computer data across a network of computers of different kinds.
* `Microsoft Backup & Restore <https://support.microsoft.com/en-us/windows/back-up-and-restore-your-pc-ac359b36-7015-4694-de9a-c5eac1ce9d9c>`_: In Windows 11, you can restore files from a backup created with Backup and Restore or File History.
* `DHS, CISA, and MS-ISAC Joint Ransomware Guide <https://www.cisa.gov/sites/default/files/publications/CISA_MS-ISAC_Ransomware%20Guide_S508C_.pdf>`_: A guide written by US federal agencies to assist with ransomware.

-----------------------------------------------
