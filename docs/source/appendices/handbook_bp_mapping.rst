..
  Created by: mike garcia
  To: index/toc for appendices

Mapping to the Handbook for Election Infrastructure Security
------------------------------------------------------------

+---------------+----------------------------------------------+---------------------------+
| Handbook BP # |	Handbook BP Title                            | Essential Guide BP        |
+---------------+----------------------------------------------+---------------------------+
|      1        | Whitelist which IPs can access the device    |                           |
+---------------+----------------------------------------------+---------------------------+
|      2        | Regularly scan the network to ensure only    | Public-Facing             |
|               | authorized devices are connected             | Network Scanning          |
+---------------+----------------------------------------------+---------------------------+
|      3        | Limit the devices that are on the same       |                           |
|               | subnet to only those devices required        |                           |
+---------------+----------------------------------------------+---------------------------+
|      4        | Only utilize approved and managed USB        | Encrypt Data at Rest      |
|               | devices with appropriate device encryption   |                           |
|               | and device authentication                    | Removable Media           |
+---------------+----------------------------------------------+---------------------------+
|      5        | Disable wireless peripheral access of        | Managing Wireless         |
|               | devices unless required and the risk is      | Networks                  |
|               | formally approved by election officials      |                           | 
+---------------+----------------------------------------------+---------------------------+
|      6        | Ensure the system is segregated from other   |                           |
|               | independent election systems and non-        |                           |
|               | election supporting systems                  |                           |
+---------------+----------------------------------------------+---------------------------+
|      7        | Deploy Network Intrusion Detection System    | Network Monitoring        |
|               | (IDS) (e.g., MS-ISAC Albert sensor) on       | and Intrusion             |
|               | internet and extranet DMZ systems            | Detection                 |
+---------------+----------------------------------------------+---------------------------+
|      8        | If wireless is required, ensure all wireless |                           |
|               | traffic use at least Advanced Encryption     |                           |
|               | Standard (AES) encryption with at least      |                           |
|               | Wi-Fi Protected Access 2 (WPA2)              |                           |
+---------------+----------------------------------------------+---------------------------+
|      9        | Use trusted certificates for any publicly-   | Website Security          |
|               | facing website                               |                           |
+---------------+----------------------------------------------+---------------------------+
|      10       | Ensure logs are securely archived            |                           |
+---------------+----------------------------------------------+---------------------------+
|      11       | On a regular basis, review logs to identify  |                           |
|               | anomalies or abnormal events                 |                           |
+---------------+----------------------------------------------+---------------------------+
|      12       | Ensure critical data are encrypted and       | Encrypt Data at Rest      |
|               | digitally signed                             |                           |
+---------------+----------------------------------------------+---------------------------+
|      13       | Ensure staff is properly trained on          | Building and              |
|               | cybersecurity and audit procedures and audit | Managing Staff            |
|               | every election in accordance with local,     |                           |
|               | state, and federal guidelines                |                           |
+---------------+----------------------------------------------+---------------------------+
|      14       | Perform system testing prior to elections    |                           |
|               | (prior to any ballot delivery), such as      |                           |
|               | acceptance testing                           |                           |
+---------------+----------------------------------------------+---------------------------+
|      15       | Ensure acceptance testing is done when       |                           |
|               | receiving or installing new/updated software |                           |
|               | or new devices                               |                           |
+---------------+----------------------------------------------+---------------------------+
|      16       | Conduct criminal background checks for all   | Building and              |
|               | staff including vendors, consultants, and    | Managing Staff            |
|               | contractors supporting the election process  |                           | 
+---------------+----------------------------------------------+---------------------------+
|      17       | Deploy application whitelisting              |                           |
+---------------+----------------------------------------------+---------------------------+
|      18       | Work with election system provider to ensure | Managing Vendors          |
|               | base system components (e.g., OS, database)  |                           |
|               | are hardened based on established industry   |                           |
|               | standards                                    |                           |
+---------------+----------------------------------------------+---------------------------+
|      19       | Regularly run a SCAP-compliant vulnerability | Public-Facing             |
|               | scanner                                      | Network Scanning          |
+---------------+----------------------------------------------+---------------------------+
|      20       | Utilize EAC certified or equivalent software | Managing Vendors          |
|               | and hardware products where applicable       |                           |
+---------------+----------------------------------------------+---------------------------+
|      21       | Store secure baseline configuration on       | Backups                   |
|               | hardened offline system and securely deploy  |                           |
|               | baseline configurations                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      22       | Utilize write once media for transferring    | Removable Media           |
|               | critical system files and system updates.    |                           |
|               | Where it is not possible to use write-once   |                           |
|               | media, that media should be used one time    |                           |
|               | (for a single direction off transfer to a    |                           |
|               | single destination device) and securely      |                           |
|               | dispose of the media.                        |                           |
+---------------+----------------------------------------------+---------------------------+
|      23       | Maintain detailed maintenance record of all  | Asset Management          |
|               | system components                            | Managing Infrastructure   |
+---------------+----------------------------------------------+---------------------------+
|      24       | Require the use of multi-factor              | User Management           |
|               | authentication                               |                           |
+---------------+----------------------------------------------+---------------------------+
|      25       | Require users to use strong passwords (14    | User Management           |
|               | character passphrases) if multi factor       |                           |
|               | authentication is not available              |                           |
+---------------+----------------------------------------------+---------------------------+
|      26       | Limit the number of individuals with         | User Management           |
|               | administrative access to the platform and    |                           |
|               | remove default credentials                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      27       | Ensure that all devices are documented and   | Asset Management          |
|               | accounted for throughout their lifecycle     | Managing Infrastructure   |
+---------------+----------------------------------------------+---------------------------+
|      28       | Utilize tamper evident seals on all external | Asset Management          |
|               | ports that are not required for use and      |                           |
|               | electronically deactivate ports where        |                           |
|               | feasible                                     |                           |
+---------------+----------------------------------------------+---------------------------+
|      29       | Maintain an inventory of assets that should  |                           |
|               | be on the same subnet as the election system |                           |
|               | component                                    |                           |
+---------------+----------------------------------------------+---------------------------+
|      30       | Establish and follow rigorous protocol for   | Asset Management          |
|               | installing tamper evident seals and          |                           |
|               | verifying their integrity upon removal       |                           |
+---------------+----------------------------------------------+---------------------------+
|      31       | Conduct load and stress tests for any        |                           |
|               | transactional related systems to ensure the  |                           |
|               | ability of the system to mitigate potential  |                           |
|               | DDoS type attacks                            |                           |
+---------------+----------------------------------------------+---------------------------+
|      32       | Limit the use of personally identifiable     | Endpoint Protection       |
|               | information. When it is required, ensure     |                           |
|               | that that it is properly secured and staff   |                           |
|               | with access are properly trained on how to   |                           |
|               | handle it.                                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      33       | Conduct mock elections prior to major        | Exercising Plans          |
|               | elections to help eliminate gaps in process  |                           |
|               | and legal areas                              |                           |
+---------------+----------------------------------------------+---------------------------+
|      34       | Identify and maintain information on network | Managing Vendors          |
|               | service providers and third-party companies  |                           |
|               | contacts with a role in supporting election  |                           |
|               | activities                                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      35       | Implement a change freeze prior to peak      |                           |
|               | election periods for major elections         |                           |
+---------------+----------------------------------------------+---------------------------+
|      36       | Prior to major elections, conduct in person  |                           |
|               | site audits to verify compliance to security |                           |
|               | policies and procedures                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      37       | Work with vendors to establish and follow    | Managing Vendors          |
|               | hardening guidance for their applications    |                           |
+---------------+----------------------------------------------+---------------------------+
|      38       | Ensure logging is enabled on the system      |                           |
+---------------+----------------------------------------------+---------------------------+
|      39       | Use automated tools to assist in log         |                           |
|               | management and where possible ensure logs    |                           |
|               | are sent to a remote system                  |                           |
+---------------+----------------------------------------------+---------------------------+
|      40       | Where feasible, utilize anti-malware         | Endpoint Protection       |
|               | software with centralized reporting          |                           |
+---------------+----------------------------------------------+---------------------------+
|      41       | Ensure only required ports are open on the   | Firewalls and Port        |
|               | system through regular port scans            | Restrictions              |
+---------------+----------------------------------------------+---------------------------+
|      42       | Where feasible, implement host-based         | Firewalls and Port        |
|               | firewalls or port filtering tools            | Restrictions              |
+---------------+----------------------------------------------+---------------------------+
|      43       | Verify software updates and the validity of  | Software Updates          |
|               | the code base through the use of hashing     |                           |
|               | algorithms and digital signatures where      |                           |
|               | available                                    |                           |
+---------------+----------------------------------------------+---------------------------+
|      44       | Ensure vendors distribute software packages  | Manage Remote Connections |
|               | and updates using secure protocols           | Software Updates          |
+---------------+----------------------------------------------+---------------------------+
|      45       | Maintain a chain of custody for all core     | Asset Management          |
|               | devices                                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      46       | All remote connection to the system will use | Manage Remote             |
|               | secure protocols (TLS, IPSEC)                | Connections               |
+---------------+----------------------------------------------+---------------------------+
|      47       | Users will use unique user IDs               | User Management           |
+---------------+----------------------------------------------+---------------------------+
|      48       | Use a dedicated machine for administrative   |                           |
|               | tasks to separate day to day functions from  |                           |
|               | other security critical functions (For some  |                           |
|               | components this may not be practical to      |                           |
|               | implement)                                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      49       | Ensure that user activity is logged and      | User Management           |
|               | monitored for abnormal activities            |                           |
+---------------+----------------------------------------------+---------------------------+
|      50       | Regularly review all accounts and disable    | User Management           |
|               | any account that can’t be associated with a  |                           |
|               | process or owner                             |                           |
+---------------+----------------------------------------------+---------------------------+
|      51       | Establish a process for revoking system      | User Management           |
|               | access immediately upon termination of       |                           |
|               | employee or contractor                       |                           |
+---------------+----------------------------------------------+---------------------------+
|      52       | Ensure that user credentials are encrypted   | User Management           |
|               | or hashed on all platforms                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      53       | Ensure all workstations and user accounts    |                           |
|               | are logged off after a period of inactivity  |                           |
+---------------+----------------------------------------------+---------------------------+
|      54       | Ensure your organization has a documented    | Building and              |
|               | Acceptable Use policy that users are aware   | Managing Staff            |
|               | of which details the appropriate uses of the |                           |
|               | system                                       |                           |
+---------------+----------------------------------------------+---------------------------+
|      55       | For data transfers that utilize physical     | Asset Management          |
|               | transmission, utilize tamper evident seals   | Removable Media           |
|               | on the exterior of the packaging             |                           |
+---------------+----------------------------------------------+---------------------------+
|      56       | Disable wireless peripheral access of        | Managing Wireless         |
|               | devices                                      | Networks                  |
+---------------+----------------------------------------------+---------------------------+
|      57       | Ensure staff is properly trained on          | Building and              |
|               | cybersecurity and audit procedures and audit | Managing Staff            |
|               | every election in accordance with local,     |                           |
|               | state, and federal guidelines                |                           |
+---------------+----------------------------------------------+---------------------------+
|      58       | Conduct criminal background checks for all   | Building and              |
|               | staff including vendors, consultants and     | Managing Staff            |
|               | contractors supporting the election process  |                           | 
+---------------+----------------------------------------------+---------------------------+
|      59       | Ensure staff is properly trained for         | Building and              |
|               | reconciliation procedures for the pollbooks  | Managing Staff            |
|               | to the voting systems and reconcile every    |                           |
|               | polling place and voter record in accordance |                           |
|               | with local, state, and federal guidelines    |                           |
+---------------+----------------------------------------------+---------------------------+
|      60       | Store secure baseline configuration on       | Backups                   |
|               | hardened offline system and securely deploy  |                           |
|               | baseline configurations                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      61       | Work with the vendor to deploy application   |                           |
|               | whitelisting                                 |                           |
+---------------+----------------------------------------------+---------------------------+
|      62       | Utilize the most up-to-date and certified    | Managing Vendors          |
|               | version of vendor software                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      63       | Utilize write once media for transferring    | Removable Media           |
|               | critical system files and system updates.    |                           |
|               | Where it is not possible to use write-once   |                           |
|               | media, that media should be used one time    |                           |
|               | (for a single direction off transfer to a    |                           |
|               | single destination device) and securely      |                           |
|               | dispose of the media.                        |                           |
+---------------+----------------------------------------------+---------------------------+
|      64       | Only use the devices for election related    |                           |
|               | activities                                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      65       | Maintain detailed maintenance records of all | Asset Management          |
|               | system components                            | Managing Infrastructure   |
+---------------+----------------------------------------------+---------------------------+
|      66       | Limit the number of individuals with         | User Management           |
|               | administrative access to the platform and    |                           |
|               | remove default credentials                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      67       | Utilize tamper evident seals on all external | Asset Management          |
|               | ports that are not required for use          |                           |
+---------------+----------------------------------------------+---------------------------+
|      68       | Ensure that all devices are documented and   | Asset Management          |
|               | accounted for throughout their lifecycle     | Managing Infrastructure   |
+---------------+----------------------------------------------+---------------------------+
|      69       | Establish and follow rigorous protocol for   | Asset Management          |
|               | installing tamper evident seals and          |                           |
|               | verifying their integrity upon removal       |                           |
+---------------+----------------------------------------------+---------------------------+
|      70       | Perform system testing prior to elections    |                           |
|               | (prior to any ballot delivery), such as      |                           |
|               | logic and accuracy testing                   |                           |
+---------------+----------------------------------------------+---------------------------+
|      71       | Ensure acceptance testing is done when       |                           |
|               | receiving or installing new or updated       |                           |
|               | software or new devices                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      72       | Conduct mock elections prior to major        | Exercising Plans          |
|               | elections to help eliminate gaps in process  |                           |
|               | and legal areas                              |                           |
+---------------+----------------------------------------------+---------------------------+
|      73       | Identify and maintain information on network | Incident Response         |
|               |  service providers and third-party companies |                           |
|               |  contacts with a role in supporting election | Managing Vendors          |
|               |  activities                                  |                           |
+---------------+----------------------------------------------+---------------------------+
|      74       | Implement a change freeze prior to peak      |                           |
|               | election periods for major elections         |                           |
+---------------+----------------------------------------------+---------------------------+
|      75       | Prior to major elections, conduct in person  |                           |
|               | site audits to verify compliance to security |                           |
|               | policies and procedures                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      76       | Verify software updates and the validity of  | Software Updates          |
|               | the code base through the use of hashing     |                           |
|               | algorithms and digital signatures where      |                           |
|               | available                                    |                           |
+---------------+----------------------------------------------+---------------------------+
|      77       | Ensure the use of unique user IDs            | User Management           |
+---------------+----------------------------------------------+---------------------------+
|      78       | Ensure individuals are only given access to  | User Management           |
|               | the devices they need for their job          |                           |
+---------------+----------------------------------------------+---------------------------+
|      79       | Maintain a chain of custody for all core     | Asset Management          |
|               | devices                                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      80       | Ensure all workstations and user accounts    |                           |
|               | are logged off after a period of inactivity  |                           | 
+---------------+----------------------------------------------+---------------------------+
|      81       | Regularly review all authorized individuals  | User Management           |
|               | and disable any account that can’t be        |                           |
|               | associated with a process or owner           |                           |
+---------------+----------------------------------------------+---------------------------+
|      82       | Ensure your organization has a documented    | Building and              |
|               | Acceptable Use policy that users are aware   | Managing Staff            |
|               | of which details the appropriate uses of the |                           |
|               | system                                       |                           |
+---------------+----------------------------------------------+---------------------------+
|      83       | Use secure protocols for all remote          | Manage Remote             |
|               | connections to the system (TLS, IPSEC)       | Connections               |
+---------------+----------------------------------------------+---------------------------+
|      84       | Ensure critical data is encrypted and        | Encrypt Data at Rest      |
|               | digitally signed                             |                           |
+---------------+----------------------------------------------+---------------------------+
|      85       | Ensure the use of bidirectional              |                           |
|               | authentication to establish trust between    |                           |
|               | the sender and receiver                      |                           |
+---------------+----------------------------------------------+---------------------------+
|      86       | For data transfers that utilize physical     | Asset Management          |
|               | transmission utilize tamper evident seals on |                           |
|               | the exterior of the packaging                |                           |
+---------------+----------------------------------------------+---------------------------+
|      87       | Conduct criminal background checks for all   | Building and              |
|               | staff including vendors, consultants and     | Managing Staff            |
|               | contractors supporting the election process  |                           | 
+---------------+----------------------------------------------+---------------------------+
|      88       | Track all hardware assets used for           | Asset Management          |
|               | transferring data throughout their lifecycle | Managing Infrastructure   |
+---------------+----------------------------------------------+---------------------------+

------------------