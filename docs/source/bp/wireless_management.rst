..
  Created by: mike garcia
  To: managing wireless networks

.. |bp_title| replace:: Managing Wireless Networks

|bp_title|
----------------------------------------------

Wireless networks are a critical piece of modern connectivity. In the election environment, some systems, like voting machines, are never connected to a wireless network. Others, like e-pollbooks, often have to be to on a wireless network to properly update voter rolls. Some jurisdictions use wireless networks to transmit election results on election night.

There's also the day-to-day administration of the elections that occur on regular workstations used by employees throughout an election office. These may use wired or wireless connections and have access to private networks or the internet.

Good cybersecurity outcomes require proper management of the wireless networks and connections in offices and polling places.

Goals
*****

#. Protect all wireless networks with basic wireless security practices (|Maturity1| maturity)
#. Deploy additional tools and measures to limit risk (|Maturity2| maturity)
#. Deploy mutual MFA for wireless access (|Maturity3| maturity)

Actions
*******

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&

For those organizations operating at a |Maturity1| maturity, the important thing is to keep it simple. Avoid using wireless in risky scenarios, such as transmitting election results without the technical support of a state agency or other technical body providing guidance.

#. Use the advanced encryption standard (:term:`AES`) to encrypt wireless data.
#. Create a separate wireless network (a guest network) for personal and untrusted devices.
#. Change administrator passwords on routers and other wireless access points to a secure passphrase.
#. Change the default access passphrase for wireless networks regularly, or enable user level authentication for private networks.
#. Don't permit visitors to use your primary wireless network. Instead set up a guest network.
#. Carefully decide whether a new device will be allowed on the network; you don't need to permit every new device onto the network.
#. Keep firmware and software up to date by including your router and other access points in your :doc:`patching <patching_vuln_management>` schedule.
#. Track what's on your network.
#. Use secure network management and communication protocols (e.g., 802.1X, Wi-Fi Protected Access 2 (:term:`WPA2 <WPA>`) Enterprise or greater). All wireless access points owned and operated by the jurisdiction should use either :term:`WPA2 <WPA>` or :term:`WPA3 <WPA>` with a strong password.


|Maturity2| Maturity
&&&&&&&&&&&&&&&&&&&&

Organizations operating at a |Maturity2| maturity should take additional actions, including:

#. Maintain an inventory of authorized wireless access points to ensure rogue ones are not introduced.
#. Disable wireless access on devices if the device does not strict require wireless connectivity.
#. Disable peer-to-peer wireless network capabilities on wireless clients to prevent communication between devices that is not visible on the wireless network.

|Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&

Organizations operating at a |Maturity3| maturity should take additional actions, including:

#. Use wireless authentication protocols that require mutual, multi-factor authentication.
#. Detect wireless access points connected to the wired network.

Cost-Effective Tools
********************

* `Aircrack-ng <https://www.aircrack-ng.org>`_: Wireless security suite
* `Kismet <https://www.kismetwireless.net>`_: Wireless security and investigation
* `Wireshark <https://www.Wireshark.org>`_: Packet capture analysis

Learn More
**********

* CIS's `Mobile Security Companion Guide <https://www.cisecurity.org/blog/new-release-cis-controls-mobile-companion-guide>`_
* NIST `Special Publication 800-153 <https://csrc.nist.gov/publications/detail/sp/800-153/final>`_: Guidelines for Securing Wireless Local Area Networks (WLANs)
* NIST `Special Publication 800-94 <https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-94.pdf>`_: Guide to Intrusion Detection and Prevention Systems (IDPS)

Mapping to CIS Controls and Safeguards
**************************************

* 12.1: Ensure Network Infrastructure is Up-to-Date (|Maturity1| maturity)
* 3.10: Encrypt Sensitive Data in Transit (|Maturity2| maturity)
* 12.3: Securely Manage Network Infrastructure (|Maturity2| maturity)
* 12.6 Use of Secure Network Management and Communication Protocols (|Maturity2| maturity)

Mapping to CIS Handbook Best Practices
**************************************

* 5, 56
