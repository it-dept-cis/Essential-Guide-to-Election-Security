..
  Created by: mike garcia
  On: 2022-03-10
  To: BP for device asset management
  Last update by: mike garcia

.. |last_update| replace:: 2022-03-14

.. include:: docs/source/global_directives.rst

.. |Maturity1| replace:: Reactive
.. |Maturity2| replace:: Proactive
.. |Maturity3| replace:: Adaptive

.. |contact_email| replace:: dontknowyet@cisecurity.org
.. |bp_title| replace:: Device Asset Management

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Without a clear understanding of what computers and other technology you must protect, you’ll have a hard time ensuring everything you own is properly secured. There are many free tools that can help automate the job of inventorying and managing physical devices, and for many organizations simple tools like spreadsheets are good enough.

Goals
**********************************************

#.	Maintain records of all hardware assets (computers and other technology) throughout their lifecycle
#.	Have an understand of where that hardware is at all times
#.	Know when maintenance or related alterations are conducted and by whom
#.	Properly protect assets from loss, theft, and tampering
#.	Remove unauthorized assets from networks and physical locations
#.	Understand chain of custody and how to maintain it


Mappings to CIS Controls and Safeguards
**********************************************

- 1.1	Establish and Maintain Detailed Enterprise Asset Inventory
- 1.2	Address Unauthorized Assets
- 1.3	Utilize an Active Discovery Tool
- 1.4	Use Dynamic Host Configuration Protocol (DHCP) Logging to Update Enterprise Asset Inventory


Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

Reactive Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For those organizations operating at a Reactive maturity, the important thing is to keep it simple. You need to know what physical assets you have, where they are, how they’re used, how they’re protected, and how they’re maintained.

If you have a fewer than a couple dozen of assets to track, it’s probably easiest to do so with a table or spreadsheet. You can do this on paper, though it’s best to also maintain a digital records that you can backup. Even if your county maintains these records, its best to do so yourself as you’re ultimately accountable for what happens in your environment.

**do we just refer folks to the SME guide or do we copy the info here?**

Proactive and Adaptive Maturites
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

Have a question, suggestion, recommendation, or correction? Contact us at |contact_email|

*This page last updated on |last_update|.*
