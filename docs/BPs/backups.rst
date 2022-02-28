..
  Created by: mike garcia
  On: 2022-02-27
  To: Backups. Derived largely from dec 2018 spotlight

.. |contact_email| replace:: dontknowyet@cisecurity.org
.. |bp_title| replace:: Backups
.. |build_date| date:: %Y-%m-%d

The Essential Guide to Election Security
==============================================
*Best Practice:* |bp_title|
----------------------------------------------

Backups are necessary due to the constant threat of modification or erasure of data due to accidental deletions, malware, and ransomware, natural disasters, or other events.

Backups also play a crucial role in expediting the recovery from malicious cyber activity allowing the restoration of a system to a reliable state that is free of malware infections and retains the original data. Rebuilding or reimaging an infected system from a known good backup or fresh operating system installation is a common best practice in incident response. For instance, if an elections network is compromised due to malware, restoring systems from a clean, uncompromised backup will allow the system to be quickly remediated and put back into production without the work of identifying and ensuring the removal of all possible malicious files.


Goals
**********************************************

#.	Create a procedure for backups
#.	Implement automated backups
#.  Protect backups
#.  Test your recovery plan

Mappings to CIS Controls and Safeguards
**********************************************

- 11.1:  Establish and maintain a data recovery process. In the process, address the scope of data recovery activities, recovery prioritization, and the security of backup data. Review and update documentation annually, or when significant enterprise changes occur that could impact this Safeguard. 
- 11.2:  Perform automated backups of in-scope enterprise assets. Run backups weekly, or more frequently, based on the sensitivity of the data.
- 11.3:  Protect recovery data with equivalent controls to the original data. Reference encryption or data separation, based on requirements.
- 11.4:  Establish and maintain an isolated instance of recovery data. Example implementations include, version controlling backup destinations through offline, cloud, or off-site systems or services.
- 11.5:  Test backup recovery quarterly, or more frequently, for a sampling of in-scope enterprise assets.

Actions
**********************************************

For |bp_title|, the necessary actions are vary by maturity as detailed below.

Reactive Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

For organizations operating at a Reactive Maturity, 

Proactive Maturity and Adaptive Maturity
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

[All the guidance and such]

Cost-Effective Tools
**********************************************

•	[tool]: [description][(link)]
•	[tool]: [description][(link)]

Terms
**********************************************

[links to glossary or has defs embedded…need to see if it’s possible to do that dynamically in github]

Learn More
**********************************************
•	[links to other random resources or knowledge or any relevant knowledge base entry

-----------------------------------------------

Have a question, suggestion, recommendation, or correction? Contact us at |contact_email|!

*This page last updated on |build_date|.*
