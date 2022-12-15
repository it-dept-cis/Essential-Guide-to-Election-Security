..
  Created by: mike garcia
  To: remake of generalized election architecture section of the Handbook

Election Results Reporting and Publishing
*****************************************

After voting is completed, results must be communicated both internally and to the public. The approach to doing this varies widely but the goal is the same: getting accurate results out as quickly as possible. The time it takes to do this depends on many factors, including state laws around where and how results are counted and when results can be posted, the length of lines when the polls close, technical specific of reporting, and factors like whether there are multiple time zones in a jurisdiciton. For instance, a state may specify that mail in ballots cannot even be opened until after polls close, which can create a signficint lag in results reporting.

This section focuses on election night reporting, which involves unofficial results.

The inputs to election results reporting and publishing are tabulated votes, as described in the previous section. The systems used for reporting and publishing are likely networked, and, in many cases, have public facing websites or application program interfaces (APIs).

The outputs are the unofficial election results, typically published on a website, often in multiple formats such as extensible markup language (XML), hypertext markup language (HTML), portable document format (PDF), and comma-separated values (CSV). There is likely a direct and persistent network connection between the published site and the internet, though the official record of the results may be kept on a system that is not persistently connected to the internet.

Risks and threats
&&&&&&&&&&&&&&&&&&&&&&&&&&&&

As noted earlier, the consequences of an attack that would impact unofficial election results reporting and publishing could be significant, resulting in loss of confidence in the correctly reported election results when they are finally posted. The primary risks to election reporting and publishing, when connected devices are used to transmit data and communicate results, are similar to those of other COTS systems. Such risks and threats include:

* Risks associated with established (whether persistent or intermittent) internet connectivity,
* Network connections with other internal systems, some of which may be owned or operated by other organizations or authorities,
* Security weaknesses in the underlying COTS products, whether hardware or software,
* Security weaknesses in proprietary products, whether hardware or software,
* Errors in properly managing authentication and access control for authorized users,
* Difficulty associated with finding, and rolling back, improper changes found after the fact, and
* Infrastructure- and process-related issues associated with backup and auditing.


How these components connect
&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Depending on the approach to submitting tabulated votes, the reporting component may be network connected. The publishing component is almost certainly network connected, but may be indirectly connected, depending on the implementation.

.. table:: Connection Types for Vote Tabulation
   :widths: auto

   ===================================  ============================================================================
   Connectedness                        System Type and Additional Information
   ===================================  ============================================================================
   Network Connected                    In some cases, election night reporting will be network connected, whether through a wired or wireless connection. The publishing component of election night reporting is almost certainly network connected, whether through a wired or wireless connection.
   Indirectly Connected                 If the election night reporting process is not network connected, it is indirectly connected through removable media.
   Not Connected                        Not applicable.
   Additional transmission-based risks  Not applicable.
   ===================================  ============================================================================
