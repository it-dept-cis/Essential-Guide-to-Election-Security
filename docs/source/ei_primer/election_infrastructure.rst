..
  Created by: mike garcia
  To: remake of generalized election architecture section of the Handbook

*This section draws from the Handbook for Election Infrastructure Security. It is an informative section to help understand and conceptualize how the various election technology components work and interact.*

A Primer on Election Infrastructure
-----------------------------------

There are many flavors of elections infrastructure, both from a technology and a process perspective. This is true far beyond just the different types of vote capture and vote tabulation devices. That said, many experts have studied the election processes at length, and there are several fundamental components common to nearly all elections systems.

In some jurisdictions, the owner of various aspects of the architecture may differ, but the fundamentals of the types of systems used to perform the task are generally the same. For that reason, many of the best practices associated with those systems will closely follow IT security best practices, though there are often additional business processes and practices that help mitigate risk.

.. figure:: /_static/generalized_election_architecture.png
   :width: 90%
   :alt: Graphic showing a generalized election architecture with data flow chart

Many of the components in elections infrastructure are built on general purpose computing machines, such as traditional web servers and database platforms. While this means they are often subject to the same attacks as those in other sectors, it also means experts have identified best practices to mitigate many of the risks.

Each of these components may exist at the state level, at the local level, or both, and some will not be applicable in certain jurisdictions. Even where there is a substantial amount of legacy infrastructure—-old systems that are difficult or impossible to update—-much can be done to mitigate risks. These systems are described below and appropriate best practices and actions are provided throughout this Guide.