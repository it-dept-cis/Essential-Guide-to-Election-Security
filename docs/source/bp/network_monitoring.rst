..
  Created by: mike garcia
  To: network intrusion monitoring/detection/prevention and albert

.. |bp_title| replace:: Network Monitoring and Intrusion Detection

.. admonition:: Status
   :class: caution

   Soft Launch Draft

|bp_title|
----------------------------------------------

Intrusion Detection Systems (:term:`IDSs <IDS>`) monitor network traffic traveling into and out of networks for malicious activity. These sensors passively monitor network data traffic but do not block traffic and cannot directly affect a member network or change the actual data traversing the network. Other technologies, called Intrusion Prevention Systems (:term:`IPSs <IPS>`), can also block traffic that the sensors deem a threat.

:term:`IDSs <IDS>` monitor traffic as it flows across a network to look for matches against a set of threat signatures. If a match is found, an alert is sent for analysis and, if warranted, further action. In this way, an :term:`IDS` can provide protection against both traditional and advanced network threats, helping organizations identify malicious activity.

The :term:`EI-ISAC` offers an IDS called Albert to election offices. The Albert sensors reside on the local network, providing security alerts for cyber threats, helping organizations identify malicious cyber activity. The sensor passively monitors network data traffic; it does not block traffic and cannot negatively affect a member network or read or change the actual data traversing the network.

Under this service, the :term:`EI-ISAC` receives any alerts, analyzes them, and works with your office to take any recommended action. The :term:`EI-ISAC` can also be used to analyze historical data to retroactively search for malicious activity. While the Albert sensor is optimized for use in the state, local, tribal, and territorial governments, commercial :term:`IDS` and :term:`IPS` systems are also available.

Goals
**********************************************

#. Understand what an :term:`IDS` is and why it's important (|Maturity1| maturity)
#. Deploy an :term:`IDS` (|Maturity2| maturity)

Mappings to CIS Controls and Safeguards
**********************************************

* 13.3: Deploy a Network Intrusion Detection Solution
* 13.4: Perform Traffic Filtering Between Network Segments
* 13.8: Deploy a Network Intrusion Prevention Solution

Actions
**********************************************

For |bp_title|, the necessary actions vary by maturity as detailed below.

|Maturity1| Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

We don't recommend investing in an :term:`IDS` at the |Maturity1| maturity.

While it can provide protection in any network environment, there are more fundamental steps to take, as described in the :doc:`|Maturity1| description <maturity_bp_mapping>`.

|Maturity2| and |Maturity3| Maturities
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

#. Consider investing in an :term:`IDS` or :term:`IPS`.
   * The Albert sensor and service is a low-cost way to do this that is optimized for use in the election offices and other state, local, tribal, and territorial governments. Contact  |eiisac_email| to get information about Albert.

-----------------------------------------------
