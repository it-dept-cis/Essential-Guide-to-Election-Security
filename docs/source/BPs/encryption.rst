..
  Created by: mike garcia
  On: 2022-03-28
  To: encryption, build largely from 2018-03-30 spotlight
  Last update by: mike garcia

.. |last_update| replace:: `2022-03-28`

.. include:: docs/source/global_directives.rst

.. |Maturity1| replace:: Reactive
.. |Maturity2| replace:: Proactive
.. |Maturity3| replace:: Adaptive

.. |contact_email| replace:: dontknowyet@cisecurity.org
.. |bp_title| replace:: Encryption

*Status: draft*

*Best Practice:* |bp_title|
----------------------------------------------

Encryption is the process whereby data is converted from a readable form (i.e., plaintext), to an encoded form (i.e., ciphertext). This encoding is designed to be unintelligible except by parties that possess a key to reverse the encoding process. This reversal process is called decryption.

Encryption allows for the confidential storage and transmission of data, as well as proof that it originated with the person who claims to have sent it. Encrypting personally identifiable information (PII) with good encryption algorithms protects the data from accidental disclosure in the case of a data breach or malware infection. Elections offices may maintain a number of systems that utilize encryption and are responsible for identifying data that should be encrypted.

Data is encrypted using a mathematical algorithm that relies on keys that are typically randomly generated. The most trusted encryption algorithms are considered secure because they have been publicly available for years and have not been broken. An attack on data encrypted with a trusted encryption algorithm could take years for even the most powerful computers to break.

There are two types of encryption: asymmetric (public key) encryption and symmetric (private key) encryption. An easy way to understand these two types of encryption is two different types of lockboxes.

In the first, symmetric cryptography, you have a lockbox with one slot for a key. You make two copies of the key, and you give one to your friend. You lock the box with your copy, and when your friend comes along, they use their copy of the same key to unlock it.

The second, asymmetric cryptography, is different. It’s more like a deposit dropbox at a bank. The bank publishes the location of the dropbox (the public key), and once you drop your deposit into it, it’s secure until the bank opens the box with the one and only copy of their key (the private key). Anyone can make a deposit once they know the location of the box, but only the bank can get deposits out.

+------------------------+---------------------------------+---------------------------------+
|        Encryption Type | Asymmetric                      | Symmetric                       |
| Characteristic         |                                 |                                 |
+========================+=================================+=================================+
| Keys                   | 2 keys – public (to be shared)  | 1 key – private (secret but     |
|                        | and private (secret and         | shared between two or more      |
|                        | possessed by only 1 person)     | partners)                       |
+------------------------+---------------------------------+---------------------------------+
| Process                | The sender encrypts information | The sender encrypts information |
|                        | with recipient’s public key and | with a private key and the      |
|                        | the recipient decrypts          | recipient decrypts information  |
|                        | information with their private  | with the same private key       |
|                        | key                             |                                 |
+------------------------+---------------------------------+---------------------------------+
| Speed                  | Slower                          | Faster                          |
+------------------------+---------------------------------+---------------------------------+

Goals
**********************************************

#.	[Goal 1]
#.	[Goal 2]

Mappings to CIS Controls and Safeguards
**********************************************

- [#.#][tab][title of control]
- [#.#][tab][title of control]

Actions
**********************************************

For |bp_title|, the necessary actions are the same for all maturity levels.

Work with those who provide IT infrastructure, whether vendors or your own IT staff, to implement encryption for all sensitive data.

Implement encryption when data is at rest (e.g., stored in a database or on a device) and in transit (e.g., sending through email) and ensure your election office’s adherence to encryption standards.

The National Institute of Standards and Technology (NIST) _`Special Publication 800-175B <https://csrc.nist.gov/publications/detail/sp/800-175b/rev-1/final>` provides the U.S. federal requirements for encryption standards to secure data at different sensitivity and classification levels.

NIST _`Special Publication 800-122 <https://csrc.nist.gov/publications/detail/sp/800-122/final>` provides the U.S. federal requirements for protecting the confidentiality of personal information.

Cost-Effective Tools
**********************************************

•	[tool]: [description][(link)]
•	[tool]: [description][(link)]

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************
•	[links to other random resources or knowledge or any relevant knowledge base entry]

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |contact_email|.

This page last updated on |last_update|.
