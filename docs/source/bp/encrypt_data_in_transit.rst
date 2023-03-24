..
  Created by: mike garcia
  To: encrypt data in transit to address gap

.. |bp_title| replace:: Encrypt Data in Transit

|bp_title|
----------------------------------------------

Any data that is being actively transferred, termed "data in transit," can present substantial risks for election offices. One of the biggest risks to election integrity occurs when transferring ballot definition files, ballot PDFs, and other such data between otherwise well-protected devices.

An election offices will often move data between its own systems and between its systems and those of vendors or other partners. An important example is transferring ballot PDFs to a commercial printer that produces the paper ballots for an upcoming eleciton. 

The most important thing to know about encrypting data in transit is that the common ways you transfer data are typically easily distinguished between encrypted and unencrypted, or secure and insecure, implementations. These different implementations are called protocols. For instance, you should never transfer important data (election data, user credentials, or the like) via a website that starts with HTTP; it should always start with HTTPS. 

Encrypted data transfer protocols are ubiquitous; you just need to make sure you and whomever you're exchanging data with use them.

Goals
*****

#. Use encrypted protocols when transferring all sensitive data (|Maturity1| maturity)
#. Ensure vendors and other partners encrypt-in-transit (|Maturity1| maturity)

Actions
*******

For |bp_title|, the necessary actions are the same for all maturity levels.

.. _encrypt-data-in-transit-all-maturities:

#. Use encrypted data transfer protocols for all sensitive data. 

   * Use HTTPS, not HTTP
   * Use FTPS, SFTP, SCP, or WebDAV over HTTPS, not FTP or RCP
   * Use SSH2, not Telnet
   * Use RDP, not VNC
 
#. Use the highest version of these protocols compatible with your systems, for instance TLS v1.2 or 1.3, not TLS 1.1 or 1.0.
#. Set defaults for these protocols and versions wherever possible throughout your systems.
#. Impose the same encryption requiremens on vendors and other partners as you use yourselves.

   * You can use the :ref:`managing vendors <managing_vendors>` best practices to help implement appropriate best practices across all of your vendors. 

.. _encrypt-data-at-rest-cost-effective-tools:

Cost-Effective Tools
********************

* `GCA Cybersecurity Toolkit for Elections: Update Your Defenses <https://gcatoolkit.org/elections/update-your-defenses/>`_: A toolbox with links to free tools relevant to this best practice
* `Bitlocker <https://technet.microsoft.com/en-us/library/cc732774(v=ws.11).aspx>`_: Built-in encryption for supported Microsoft® Windows devices.

Mapping to CIS Controls and Safeguards
**************************************

* 3.10: Encrypt Sensitive Data in Transit
* 15.4: Ensure Service Provider Contracts Include Security Requirements

Mapping to CIS Handbook Best Practices
**************************************

* 8, 12, 84
