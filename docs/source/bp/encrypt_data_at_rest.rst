..
  Created by: mike garcia
  To: encryption, build largely from 2018-03-30 spotlight

.. |bp_title| replace:: Encrypt Data at Rest

|bp_title|
----------------------------------------------

Any data that is not being actively transferred can be referred to "data at rest." This includes data residing on hard drives, USB sticks, and with third-party cloud service providers. Encryption allows for data at rest to be properly secured. For instance, encrypting personally identifiable information (PII) with strong encryption algorithms protects the data from accidental disclosure in the case of a data breach.

Elections offices may maintain a number of systems that must use encryption and are responsible for identifying data that should be encrypted.

In modern laptops, desktops, and server environments, encryption capabilities of some form are often built into the software and hardware stack. These capabilities may be enabled by default or will need to be properly configured. Third-party encryption utilities may also be needed to encrypt specific data, such as within an application, database, or a USB device.


Goals
*****

#. Enable encryption for laptops, desktops, servers, and mobile devices, known as full-disk encryption (|Maturity1| maturity)
#. Encrypt backups (|Maturity1| maturity)
#. Encrypt removable devices, where practical, such as with USB devices (|Maturity2| maturity)

Actions
*******

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _encrypt-data-at-rest-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&

#. Enable encryption, often called full-disk encyrption, on all devices that have encryption technologies built into the device. 

   * You can use the |Maturity1| maturity :ref:`Asset Protection worksheet <cybersecurity-action-worksheets>` as a template to track your work. 
   * The :ref:`cost effective tools <encrypt-data-at-rest-cost-effective-tools>` section below may help, depending on the types of systems you have in your environment.

#. Encrypt backups. Use the :doc:`backups <backups>` best practice as a guide.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Organizations operating at a |Maturity2| or |Maturity3| maturity should take additional actions, including:

#. Work with those who provide IT infrastructure, whether vendors or your own IT staff, to implement encryption for all sensitive data.
#. Implement encryption when data is at rest (e.g., stored in a database or on a device) and in transit (e.g., sending through email) and ensure all encryption meets your election office’s adherence to encryption standards.

The National Institute of Standards and Technology (:term:`NIST`) `Special Publication 800-175B <https://csrc.nist.gov/publications/detail/sp/800-175b/rev-1/final>`_ provides the U.S. federal requirements for encryption standards to secure data at different sensitivity and classification levels.

NIST `Special Publication 800-122 <https://csrc.nist.gov/publications/detail/sp/800-122/final>`_ provides the U.S. federal requirements for protecting the confidentiality of personal information.

.. _encrypt-data-at-rest-cost-effective-tools:

Cost-Effective Tools
********************

* `GCA Cybersecurity Toolkit for Elections: Update Your Defenses <https://gcatoolkit.org/elections/update-your-defenses/>`_: A toolbox with links to free tools relevant to this best practice
* `Bitlocker <https://technet.microsoft.com/en-us/library/cc732774(v=ws.11).aspx>`_: Built-in encryption for supported Microsoft® Windows devices.
* `FileVault <https://support.apple.com/en-us/HT204837>`_: Built-in encryption for MacOS devices.
* `Veracrypt <https://www.veracrypt.fr/en/How%20to%20Back%20Up%20Securely.html>`_: Open-source, free full disk encryption utility.
* `EaseUS <https://www.easeus.com/backup-software/tb-free.html>`_: This free program can encrypt system images.

Mapping to CIS Controls and Safeguards
**************************************

* 3.6: Encrypt Data on End-User Devices
* 3.9: Encrypt Data on Removable Media
* 3.11: Encrypt Sensitive Data at Rest
* 11.3: Protect Recovery Data

Mapping to CIS Handbook Best Practices
**************************************

* 4, 12, 84
