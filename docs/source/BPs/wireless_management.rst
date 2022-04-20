..
  Created by: mike garcia
  To: managing wireless networks

.. |bp_title| replace:: Managing Wireless Networks

*Best Practice:* |bp_title|
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

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For those organizations operating at a |Maturity1| maturity, the important thing is to keep it simple. Avoid using wireless in risky scenarios, such as transmitting election results without the technical support of a state agency or other technical body providing guidance.

#. Leverage the Advanced Encryption Standard (AES) to Encrypt Wireless Data
#. Create Separate Wireless Network for Personal and Untrusted Devices

|Maturity2| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

With at least some technical staff, you can

#. Disable Wireless Access on Devices if Not Required
#. Maintain an Inventory of Authorized Wireless Access Points
#. Detect Wireless Access Points Connected to the Wired Network
#. Disable Peer-to-Peer Wireless Network Capabilities on Wireless Clients
#. Disable Wireless Peripheral Access of Devices

|Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

At the Adaptive maturity, you should be

#. Limit Wireless Access on Client Devices
#. Use a Wireless Intrusion Detection System
#. Use Wireless Authentication Protocols that Require Mutual, Multi-Factor Authentication



For |bp_title|, the necessary actions are the same for all maturity levels.

#. Change administrator passwords on routers and other wireless access points to a secure passphrase.
#. Change the default access passphrase for wireless networks regularly, or enable user level authentication for private networks.
#. Don't permit visitors to use your primary wireless network. Instead set up a separate network or enable a guest network.
#. Carefully decide whether a new device will be allowed on the network; you don't need to permit every new device onto the network.
#. Keep firmware and software up to date by including your router and other access points in your :doc:`patching` schedule.
#. Use :doc:`encryption` for all network traffic.
#. Track what's on your network.
#. Use secure network management and communication protocols (e.g., 802.1X, Wi-Fi Protected Access 2 (WPA2) Enterprise or greater).

Cost-Effective Tools
**********************************************

* [tool]: [description][(link)]
* [tool]: [description][(link)]

Learn More
**********************************************
* [links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------
