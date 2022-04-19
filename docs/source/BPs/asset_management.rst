..
  Created by: mike garcia
  To: BP for device asset management

.. |bp_title| replace:: Asset Management

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Without a clear understanding of what computers and other technology you must protect, you’ll have a hard time ensuring everything you own is properly secured. There are many free tools that can help automate the job of inventorying and managing physical devices, and for many organizations simple tools like spreadsheets are good enough.

Goals
**********************************************

#.	Maintain records of all assets (hardware, software, cloud platforms) throughout their lifecycle
#.	Know the physical location of hardware at all times
#.	Know when maintenance or related alterations are conducted and by whom
#.	Properly protect assets from loss, theft, and tampering
#.	Remove unauthorized assets from networks and physical locations
#.	Understand chain of custody and how to maintain it


Mappings to CIS Controls and Safeguards
**********************************************

- 1.1:	Establish and Maintain Detailed Enterprise Asset Inventory (Reactive)
- 1.2:	Address Unauthorized Assets (Reactive)
- 1.3:	Utilize an Active Discovery Tool (Proactive)
- 1.4:	Use Dynamic Host Configuration Protocol (DHCP) Logging to Update Enterprise Asset Inventory (Adaptive)


Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

ACTION 1: Create an inventory of all state and county technology owned and operated in support of election activities. This includes hardware assets, software, and cloud service providers such as laptops, software suites (e.g., Adobe), and email providers.

ACTION 2: Investigate unknown assets discovered during the inventory process. Remove assets that should not be attached to the network.

For those organizations operating at a Reactive maturity, the important thing is to keep it simple. You need to know what physical assets you have, where they are, how they’re used, how they’re protected, and how they’re maintained. Understanding this information will help you properly defend your network and other IT assets.

If you have a fewer than a couple dozen of assets to track, it’s probably easiest to do so with a table or spreadsheet. You can do this on paper, though it’s best to also maintain a digital records that you can backup. Even if your county maintains these records, its best to do so yourself as you’re ultimately accountable for what happens in your environment. Accordingly, contractor systems should be included in your inventory. Note that this inventory will contain sensitive information from a security perspective that should not be shared within untrusted parties.

**do we just refer folks to the SME guide or do we copy the info here?**

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Organizations operating at a Proactive or Adaptive maturity should take additional actions, including maintaining digital inventory records, applying asset tags, and implementing software tools to discover physical devices on your networks.

Enterprise tools exist to automate this process. If you are at a Proactive or Adaptive maturity, you should be implementing one of them.

Ensure the inventory records the network address (if static), hardware address, machine name, data asset owner, department for each asset, and whether the asset has been approved to connect to the network. For mobile end-user devices, MDM type tools can support this process, where appropriate. This inventory includes assets connected to the infrastructure physically, virtually, remotely, and those within cloud environments. Additionally, it includes assets that are regularly connected to the enterprise’s network infrastructure, even if they are not under control of the enterprise. Review and update the inventory of all enterprise assets bi-annually, or more frequently.

Cost-Effective Tools
**********************************************

•	CIS Enterprise Asset Inventory Worksheet: An excel workbook suitable for small operations a limited number of assets (https://www.cisecurity.org/white-papers/cis-hardware-and-software-asset-tracking-spreadsheet/)
•	Nmap: Famous multipurpose network scanner, used by system administrators and hackers across the world to identify which devices are connected to your network (https://nmap.org/)
•	ZenMap: Easy-to-use graphic user interface for Nmap (https://nmap.org/zenmap/)
•	Spiceworks: Free IT inventory and asset management software to identify devices and software on your network (https://www.spiceworks.com/)


Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************
•	[links to other random resources or knowledge or any relevant knowledge base entry

-----------------------------------------------
