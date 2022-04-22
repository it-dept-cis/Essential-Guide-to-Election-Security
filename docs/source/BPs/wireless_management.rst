..
  Created by: mike garcia
  To: managing wireless networks

.. |bp_title| replace:: Managing Wireless Networks

|bp_title|
----------------------------------------------

Wireless networks are a critical piece of modern connectivity. In the election environment, some systems, like voting machines, are never connected to a wireless network. Others, like e-pollbooks, often have to be to on a wireless network to properly update voter rolls. Some jurisdictions may even use wireless networks to transmit election results on election night.

There's also the day-to-day administration of the elections that occur on regular workstations used by employees throughout an election office. These may use wired or wireless connections and have access to private networks or the internet.

Good cybersecurity outcomes require proper management of the wireless networks and connections in your offices and polling places.

Goals
**********************************************

#.  Understand situations where the use of wireless networks introduces additional risk.
#.  Understand how to protect wireless networks

Mappings to CIS Controls and Safeguards
**********************************************

* 3.10: Encrypt Sensitive Data in Transit
* 12.1: Ensure Network Infrastructure is Up-to-Date
* 12.3: Securely Manage Network Infrastructure  [#.#] [title of control]
* 12.6 Use of Secure Network Management and Communication Protocols 

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For those organizations operating at a |Maturity1| maturity, the important thing is to keep it simple. Avoid using wireless in risky scenarios, such as transmitting election results without the technical support of a state agency or other technical body providing guidance.

#. Leverage the advanced encryption standard (AES) to encrypt wireless data.
#. Create separate wireless network for personal and untrusted devices.
#. Change administrator passwords on routers and other wireless access points to a secure passphrase.
#. Change the default access passphrase for wireless networks regularly, or enable user level authentication for private networks.
#. Don't permit visitors to use your primary wireless network. Instead set up a separate network or enable a guest network.
#. Carefully decide whether a new device will be allowed on the network; you don't need to permit every new device onto the network.
#. Keep firmware and software up to date by including your router and other access points in your :doc:`patching <software_updates>` schedule.
#. Use :doc:`the encryption best practice <encryptdataatrest>` for all network traffic.
#. Track what's on your network.
#. Use secure network management and communication protocols (e.g., 802.1X, Wi-Fi Protected Access 2 (WPA2) Enterprise or greater).

All wireless access points owned and operated by the jurisdiction should utilize either WPA2 or WPA3 with a strong password.

Untrusted devices from users outside of your jurisdiction should not be provided access to the jurisdiction's primary wireless network. If they are not part of your team, they should not be on the same wireless network as jurisdiction equipment. A guest network should be used to enforce separation.

|Maturity2| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

In addition to those actions for the |Maturity1| maturity, with at least some technical staff, you should:

#. Maintain an inventory of authorized wireless access points to ensure rogue ones are not introduced.
#. Disable wireless access on devices if the device does not require access.
#. Disable peer-to-peer wireless network capabilities on wireless clients to prevent communication between devices that is not visible on the wireless network.

|Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

At the |Maturity3| maturity, you should do all of the above and:

#. Use wireless authentication protocols that require mutual, multi-factor authentication.
#. Detect wireless access points connected to the wired network.

Cost-Effective Tools
**********************************************

* [tool]: [description][(link)]
* [tool]: [description][(link)]

Learn More
**********************************************
* [links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------
