..
  Created by: mike garcia
  To: BP for device asset management

.. |bp_title| replace:: Asset Management

|bp_title|
----------------------------------------------

Without a clear understanding of what computers and other technology you must protect, you’ll have a hard time ensuring everything you own is properly secured.

There are many free tools that can help automate the job of inventorying and managing physical devices, and for many organizations simple tools like spreadsheets are good enough.

Goals
**********************************************

#. Maintain proper records of all assets (hardware, software, cloud platforms) throughout their lifecycle (|Maturity1| maturity)
#. Always know the physical location of hardware (|Maturity1| maturity)
#. Conduct maintenance and protecting assets from loss, theft, and tampering (|Maturity1| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

.. _asset-management-maturity-one:

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For those organizations operating at a |Maturity1| maturity, keep it simple. You need to know what physical assets you have, where they are, how they’re used, how they’re protected, and how they’re maintained. Understanding this information will help you properly defend your network and other IT assets.

#. Create an inventory of all state and county technology owned and operated in support of election activities. This includes hardware assets, software, and cloud service providers such as laptops, software suites (e.g., Adobe), and email providers.

   * If you have a fewer than a couple dozen of assets to track, it’s probably easiest to do so with a table or spreadsheet. You can do this on paper, though if you use paper, you should also maintain a digital records that you can backup. You can use the |Maturity1| maturity :ref:`IT Inventory Worksheets <IT-inventory-worksheets>` as a template or the `CIS Enterprise Asset Inventory Worksheet`_.
   * Even if your county maintains these records, it's best to do so yourself, as you’re ultimately accountable for what happens in your environment.
   * Contractor systems should be included in your inventory. 
   * This inventory will contain sensitive security information that should not be shared with untrusted parties.

#. Investigate unknown assets discovered during the inventory process. Remove assets that should not be attached to the network. This includes both hardware and software assets.

.. _asset-management-maturity-two-three:

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Organizations operating at a |Maturity2| or |Maturity3| maturity should take additional actions, including:

#. Maintaining digital inventory records.
#. Applying asset tags.
#. Implementing software tools to discover physical devices on your networks.
#. Allowlist authorized software to prevent unwanted software installation.

Enterprise tools exist to automate this process and if you are at a higher maturity, you should be implementing one of them.

Ensure the inventory records the network address (if static), hardware address, machine name, data asset owner, department for each asset, and whether the asset has been approved to connect to the network. For mobile end-user devices, mobile device management (:term:`MDM`) tools can support this process, where appropriate.

This inventory should include assets connected to the infrastructure physically, virtually, remotely, and those within cloud environments. Additionally, it includes assets that are regularly connected to the enterprise’s network infrastructure, even if they are not under the control of your organization. Review and update the inventory of all enterprise assets bi-annually, or more frequently.

Cost-Effective Tools
**********************************************

* `CIS Enterprise Asset Inventory Worksheet`_: An excel workbook suitable for small operations with a limited number of assets
* `Nmap <https://nmap.org/>`_: Famous multipurpose network scanner used by system administrators and hackers across the world to identify which devices are connected to your network
* `ZenMap <https://nmap.org/zenmap/>`_: Easy-to-use graphic user interface for Nmap
* `Spiceworks <https://www.spiceworks.com/>`_: Free IT inventory and asset management software to identify devices and software on your network

Mapping to CIS Controls and Safeguards
**********************************************

* 1.1: Establish and Maintain Detailed Enterprise Asset Inventory (|Maturity1| maturity)
* 1.2: Address Unauthorized Assets (|Maturity1| maturity)
* 2.3: Address Unauthorized Software (|Maturity1| maturity)
* 1.3: Utilize an Active Discovery Tool (|Maturity2| maturity)
* 2.5: Allowlist Authorized Software (|Maturity2| maturity)
* 1.4: Use Dynamic Host Configuration Protocol (DHCP) Logging to Update Enterprise Asset Inventory (|Maturity3| maturity)

Mapping to CIS Handbook Best Practices
****************************************

* 23, 27, 28, 30, 45, 55, 65, 67, 68, 69, 79, 86, 88

.. _CIS Enterprise Asset Inventory Worksheet: https://www.cisecurity.org/white-papers/cis-hardware-and-software-asset-tracking-spreadsheet/
