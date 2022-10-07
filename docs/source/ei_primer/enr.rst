..
  Created by: mike garcia
  To: remake of generalized election architecture section of the Handbook

*This section draws from the Handbook for Election Infrastructure Security. It is an informative section to help understand and conceptualize how the various election technology components work and interact.*

Election results reporting and publishing
*****************************************

After votes are tabulated, results must be communicated both internally and to the public. In any given state, this can take many forms, but, in most cases, the basic process goal remains: getting results as quickly and accurately as possible. This section focuses on election night reporting, which involves unofficial results.

The inputs to election results reporting and publishing are tabulated votes, as described in the previous section. The systems used for reporting and publishing are likely networked, and, in many cases, have public facing websites.

The outputs are the unofficial election results, typically published on a website, often in multiple formats such as extensible markup language (XML), hypertext markup language (HTML), portable document format (PDF), and comma-separated values (CSV). There is likely a direct and persistent network connection between the published site and the internet, though the official record of the results may be kept on a system that is not persistently connected to the internet.

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
