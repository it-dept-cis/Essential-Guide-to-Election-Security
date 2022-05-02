..
  Created by: mike garcia
  To: encryption, build largely from 2018-03-30 spotlight

.. |bp_title| replace:: Encrypt Data at Rest

*Best Practice:* |bp_title|
----------------------------------------------

Any data stored on a computer system that is not being actively transferred can be referred to "data at rest." This includes data residing on HDDs, SSDs, USB sticks, and even third party cloud service providers. Encryption allows for data at rest to be properly secured. For instance, encrypting personally identifiable information (PII) with strong encryption algorithms protects the data from accidental disclosure in the case of a data breach.

Elections offices may maintain a number of systems that must utilize encryption and are responsible for identifying data that should be encrypted.

In modern laptops, desktops, and server environments, encryption capabilities of some form are often built into the software and hardware stack. These capabilities may be enabled by default or will need to be properly configured. Third-party encryption utilities may also be needed to encrypt specific data, such as within an application, database, or a USB device.


Goals
**********************************************

#. Utilize full-disk encryption for laptops, desktops, servers, and mobile devices (|Maturity1| maturity)
#. Encrypt backups (|Maturity1| maturity)
#. Encrypt removable devices, where practical, such as with USB devices (|Maturity2| maturity)


Mappings to CIS Controls and Safeguards
**********************************************

* 3.6: Encrypt Data on End-User Devices
* 3.9: Encrypt Data on Removable Media
* 3.11: Encrypt Sensitive Data at Rest
* 11.3: Protect Recovery Data

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _encrypt-data-at-rest-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Enable full disk encryption on all devices that have encryption technologies built into the device. You can use the |Maturity1| maturity :ref:`Asset Protection worksheet <cybersecurity-action-worksheets>` as a template.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Work with those who provide IT infrastructure, whether vendors or your own IT staff, to implement encryption for all sensitive data.

Implement encryption when data is at rest (e.g., stored in a database or on a device) and in transit (e.g., sending through email) and ensure your election office’s adherence to encryption standards.

The National Institute of Standards and Technology (:term:`NIST`) `Special Publication 800-175B <https://csrc.nist.gov/publications/detail/sp/800-175b/rev-1/final>`_ provides the U.S. federal requirements for encryption standards to secure data at different sensitivity and classification levels.

NIST `Special Publication 800-122 <https://csrc.nist.gov/publications/detail/sp/800-122/final>`_ provides the U.S. federal requirements for protecting the confidentiality of personal information.

Cost-Effective Tools
**********************************************

* `Bitlocker <https://technet.microsoft.com/en-us/library/cc732774(v=ws.11).aspx>`_: Built-in encryption for supported Microsoft® Windows devices.
* `FileVault <https://support.apple.com/en-us/HT204837>`_: Built-in encryption for MacOS devices.
* `Veracrypt <https://www.veracrypt.fr/en/How%20to%20Back%20Up%20Securely.html>`_: Open-source, free full disk encryption utility.
* `EaseUS <https://www.easeus.com/backup-software/tb-free.html>`_: This free program can encrypt system images.

-----------------------------------------------