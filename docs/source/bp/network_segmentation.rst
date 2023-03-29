..
  Created by: mike garcia
  To: network segmentation

.. |bp_title| replace:: Segment Networks Based on Sensitivity

|bp_title|
----------------------------------------------

Network Segmentation is the practice of splitting a network into multiple sub-networks. These networks are usually designed around business needs, for example, having sub-networks for executives, finance, operations, and human resources or by keeping election functions separated from other county functions. Networks can also be separated by data sensitivity, keeping more sensitive election data separated from every day communications.

Keeping information segmented can shrink the attack surface: successful attacks on one part of a network are less likely to impact the other parts. It can also lead to performance improvements within each sub-network.

Network segmentation can be physical or logical. Physical segmentation keeps network traffic separate through devices such as firewalls and switches. Logical segmentation uses virtual networks and addressing schemes to keep traffic on its intended sub-network. 

Goals
*****

#. Know whether your election environment needs to segmented and understand the best ways to do so (|Maturity1| maturity)
#. Deploy appropriate network segmentation tools (|Maturity1| maturity)
#. Manage network segmentation appropriately (|Maturity1| maturity) 

Actions
*******

For |bp_title|, the necessary actions are the same for all maturity levels.

#. Take simple steps to segment traffic, like creating a guest wireless network and a voice network.
#. Determine your network segmentation strategy, including whether to employ physical segmentation, logical, or both.
#. Deploy a network segmentation tools appropriate for your environment, including establishing policies for firewalls and related devices.
#. Monitor and adjust policies to meet the changing needs of your organization.

Cost-Effective Tools
********************

* tk

Mapping to CIS Controls and Safeguards
**************************************

* 3.12: Segment Data Processing and Storage Based on Sensitivity
* 12.2: Establish and Maintain a Secure Network Architecture
* 12.8: Establish and Maintain Dedicated Computing Resources for All Administrative Work
* 13.4: Perform Traffic Filtering Between Network Segments

Mapping to CIS Handbook Best Practices
**************************************

* 6
