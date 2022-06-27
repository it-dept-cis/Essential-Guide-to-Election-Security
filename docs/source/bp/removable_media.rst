..
  Created by: mike garcia
  To: manage removable media

.. |bp_title| replace:: Managing Removable Media

|bp_title|
----------------------------------------------

While removable media such as :term:`USB` drives and :term:`PCMCIA` cards are going extinct in most IT environments, they are still an important tool where not some machines are not network connected.

In the election environment, the election management system and voting systems typically have no network connections and are not on the internet, so removable media remains a part of everyday life.

While keeping hardware and software off of networks can eliminate certain threats, others can be introduced by exchanging data with removable media. Election offices need to be sure to properly source and sanitize anything used to physically transfer data between machines.

Goals
**********************************************

#. Understand media sanitization (|Maturity1| maturity)
#. Effectively use removable media in the election environment (|Maturity1| maturity)

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity, as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

It's best to use removable media only once. This could mean using a :term:`CD-R`, :term:`DVD-R`, or other once-write media, but that can be difficult with today's machines.

Instead, use :term:`USB` sticks or other removable media like flash cards. If your budget can sustain it, use them once. If not, follow a media sanitization guide to reduce the risk of introducing :term:`malware` into your non-networked machines.

Also, be sure to source your removable media from trusted sources or, if you can't, the consumer market, like a big box store where there's enough volume that it would be difficult to target you as an election office. CIS's `cybermarket <https://www.cisecurity.org/services/cis-cybermarket>`_ offers :term:`USB` sticks and other products from vetted vendors.

|Maturity2| and |Maturity3| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

While following the same guidance as the |Maturity1| maturity, make removable media sanitization a part of your larger media sanitization program. `NIST SP 800-88 <https://csrc.nist.gov/publications/detail/sp/800-88/rev-1/final>`_ is the gold standard for such a program.

Cost-Effective Tools
**********************************************

* CIS's `cybermarket <https://www.cisecurity.org/services/cis-cybermarket>`_. A buying guide for EI-ISAC members, providing products from trusted vendors at discounted rates.

Mapping to CIS Controls and Safeguards
**********************************************

* 3.9: Encrypt Data on Removable Media (|Maturity1| maturity)
* 10.3: Disable Autorun and Autoplay for Removable Media (|Maturity1| maturity)
* 10.4: Configure Automatic Anti-Malware Scanning of Removable Media (|Maturity2| maturity)

Mapping to CIS Handbook Best Practices
****************************************

* 4, 22, 55, 63
