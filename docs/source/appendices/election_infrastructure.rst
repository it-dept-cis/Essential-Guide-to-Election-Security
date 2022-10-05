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

Voter registration
******************

Every state has a unique approach to voter registration—-including some states with automatic voter registration—-but there are several commonalities shared by all of them. Voter registration systems provide voters with the opportunity to establish their eligibility and right to vote, and for states and local jurisdictions to maintain each voter’s record, often including assigning voters to the correct polling location. Voter registration systems support pollbooks—paper and electronic—as well as provide information back to the voter as they verify their registration and look up polling locations and sample ballots.

The inputs to voter registration systems are registrations, removals due to ineligibility (e.g., an individual moving out of state, death of an individual), and record updates, most often due to an individual moving within the state. The outputs include facilitating voter lookups—-such as a voter verifying they are registered, seeking a sample ballot, or finding their polling place—-and transfer of voter information to pollbooks.

In each of these cases, there is a master voter database at the state level. This database is populated in one of three broad ways (lightly edited from the Election Assistance Commission's 2014 Statutory Overview):

#. A top-down system in which the data are hosted on a single, central platform of hardware and maintained by the state with data and information supplied by local jurisdictions,
#. A bottom-up system in which the data are hosted on local jurisdictions' hardware and periodically compiled to form a statewide voter registration list, or
#. A hybrid approach, which is a combination of a top-down and bottom-up system.

For all three cases, voter registration systems consist of one or more applications that leverage general-purpose computing systems built on commercial-off-the-shelf (:term:`COTS``) hardware and software. Because they use these common computing platforms, voter registration systems may be part of a shared computing system, though in many cases they are dedicated systems with dedicated software.

While jurisdictions vary in how they allow voters to apply or update their registration, in many states, the most common way voters access a registration system is through the state’s department of motor vehicles (DMV).
Additionally, voters’ connection to the voter registration system may run through direct means such as a county or state registration portal, or through indirect means like mailing in a registration on paper. To address this risk, many voter registration systems with which the voter would interact are separated from the “official,” or production, voter registration system. Periodically, a report of changes is generated and undergoes a quality assurance review that must be certified before being entered into the production system. This can substantially reduce, for instance, an online portal as a vector of attack, though the production system may still be network connected in other ways.

In general, voter registration systems exhibit the risk characteristics of a general-purpose computing system and, more specifically, any network connected database application. To properly mitigate risks, each voter registration system within a state, and links to the voter registration system, needs a comprehensive assessment of its technical characteristics and the application of appropriate security controls.

.. figure:: /_static/voter_registration_breakout.png
   :width: 90%
   :alt: Graphic showing a the components of a typical voter registration system

Types of voter registration systems
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Voter registration generally occurs in one of two ways, each of which is recorded in a statewide registration system.

#. Online registration: a website or other web application allows prospective voters to register electronically and have election officials review their registration for validity, which, if valid, is entered into the voter registration database. Same-day registration, because of the need for live updating and cross checking, usually falls into this category.
#. Paper-based registration: prospective voters submit a paper voter registration form that is reviewed by election officials and, if valid, entered into the voter registration database.

The type of voter registration employed at DMVs will vary by state—and perhaps locality—but should typically be viewed as a form of online registration.

Risks and threats
&&&&&&&&&&&&&&&&&

As noted in the previous section, the ability to access voter registration systems through the internet results in a significant increase in vulnerability and resulting risk. There are well known best practices to mitigate these risks, but the ability to attack and manipulate voter registration systems by remote means makes them a priority for strengthening of the security resilience of these components.

While attacks on voter registration systems may have a specific purpose not found outside the elections domain, the vectors for those attacks, and thus the primary risks and threats associated with voter registration systems, are similar to those of other systems running on COTS IT hardware and software, and include:

* Risks associated with established (whether persistent or intermittent) internet connectivity,
* Network connections with other internal systems, some of which may be owned or operated by other organizations or authorities,
* Security weaknesses in the underlying COTS products, whether hardware or software,
* Errors in properly managing authentication and access control for authorized users,
* Difficulty associated with finding, and rolling back, improper changes found after the fact, and
* Infrastructure- and process-related issues associated with backup and auditing.

These items must be managed to ensure proper management of voter registration systems. Because they are risks and threats shared among users of COTS products, there is a well-established set of controls to mitigate risk and thwart threats, as provided throughout this Guide and in related cyberscurity guidance such as the :doc:`CIS Controls <cis_controls>`.

How these components connect
&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Each type of voter registration, along with the master voter registration database, should have risks evaluated individually based on its type of connectivity and employ controls and best practices found throughout this Guide that correspond to the type of connectivity and are appropriate to address risks. That said, aspects of the voter registration systems, and the types that may be implemented, have general characteristics that can be classified by connectivity.

.. table:: Connection Types for Voter Registration Systems
   :widths: auto

   ==================================  =============================================================================
   Connectedness                       System Type and Additional Information
   ==================================  =============================================================================
   Network Connected                   Online Registration. In addition, the master registration database or system itself should be considered network connected. 
   Indirectly Connected                Not applicable in most voter registration implementations.
   Not Connected                       Paper-based registration.
   Additinal Transmission-based Risks  Transmission of a registration via email or fax leverages a digital component.
   ==================================  =============================================================================

Pollbooks
*********

Pollbooks assist election officials by providing voter registration information to workers at each polling location. Historically, these were binders that contained voter information and could be used to mark off voters when they arrived to vote. While paper pollbooks remain in use today, many pollbooks are electronic and aim to facilitate the check-in and verification process at in-person polling places. While this section focuses primarily on electronic pollbooks (e-pollbooks), it also recognizes that, depending on the implementation, producing paper pollbooks can carry transmission-based risks.

These e-pollbooks play a critical role in the voting process. They are necessary to ensure voters are registered and are appearing at the correct polling place, and their efficient use is necessary to ensure sufficient throughput to limit voters’ wait times. These e-pollbooks are typically dedicated software built on COTS hardware (usually a tablet) and riding on COTS operating systems, like Android or iPadOS.

The primary input to e-pollbooks is the appropriate portion of the registration database. The primary output is the record of a voter having received a ballot, and in some cases providing a token to activate the vote capture device. In some cases, for instance where same-day registration is permitted, e-pollbooks may require additional inputs and outputs to allow for election day changes.

Paper pollbooks are produced from digital records, including digital registration databases. Having taken appropriate measures to mitigate risk for voter registration components, secure transmission of voter information to a printer—whether at the state or local level, or via commercial printing services—protects the integrity of the information in printed pollbooks.

Risks and threats
&&&&&&&&&&&&&&&&&

Attacks on e-pollbooks would generally serve to disrupt the election day process by one of these three situations: 
#. Attacking the integrity of the data on the pollbook by altering the information displayed from voter rolls,
#. Disrupting the availability of the e-pollbooks themselves, or 
#. In some cases, causing issues with the vote capture device by altering an activation token. 

Any of these situations could result in confusion at the polling locations and likely a loss of confidence in the integrity of election results. A successful attack of the first variety would more likely occur in voter registration systems by deleting voters from rolls or subtly modifying information in a way that causes delays in their casting a ballot or forces them to use the provisional ballot process, but could also occur in the e-pollbooks themselves and during the transmission of data to the e-pollbook.

An e-pollbook may or may not be connected to a network. If they are network connected, they must be treated as having the risks of a network connected device, even if the functionality is not used. While threats are continually evolving, appropriate measures can be taken to address this largely known set of risks.

The primary cybersecurity-related risks to paper pollbooks come from the transmission of pollbook data to formatting and printing services. Data will typically be loaded onto an e-pollbook through a wired connection, a wireless network, or removable media such as a USB stick. To that end, risks and threats include:

* Risks associated with established (whether persistent or intermittent) internet connectivity,
* Network connections with other internal systems, some of which may be owned or operated by other organizations or authorities, including private networks for e-pollbooks,
* Security weaknesses in the underlying COTS products, whether hardware or software,
* Security weaknesses in the dedicated components, whether hardware or software,
* Errors in properly managing authentication and access control for authorized users, including permissions for connecting to networks and attaching removable media, and
* Difficulty associated with finding, and rolling back, improper changes found after the fact.

These risks must be managed to ensure proper management of pollbooks. Because most are risks and threats shared among users of COTS products more broadly than in elections, there is a well-established set of controls to mitigate risk and thwart threats.

How these components connect
&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Managing risks associated with e-pollbooks will generally fall into one of two classifications based on the way they can connect to load data and, if applicable, transmit data. Based on the type of connectivity for a given implementation, Part 3 provides mitigations for these risks.

.. table:: Connection Types for Pollbooks
   :widths: auto

   ==================================  =============================================================================
   Connectedness                       System Type and Additional Information
   ==================================  =============================================================================
   Network Connected                   Pollbook connects via a wired or wireless network 
   Indirectly Connected                Pollbook connects via a physical media connection or removable media (e.g., USB sticks and other flash media that are physically connected and disconnected to other devices).
   Not Connected                       Paper-based pollbooks.
   Additinal Transmission-based Risks  Transmission of data for paper-based pollbooks for formatting or printing.
   ==================================  =============================================================================

State and Local Election Management Systems
*******************************************

States and local jurisdictions generally have established, persistent Election Management Systems (EMSs) that handle all backend activities for which those officials are responsible. Each state has an EMS, and each local jurisdiction will typically have a separate EMS that may, but will not always, connect to the state’s system. The extent to which the two systems are integrated, if at all, varies greatly.

For the most part, a local EMS is used to design or build ballots, program the election database, and report results. A state EMS typically does a wide variety of things including election night reporting and military and overseas ballot tracking.

An EMS will also typically include vote tabulation. For the purposes of this handbook, vote tabulation is broken out into its own section.

EMSs can have a wide variety of inputs and outputs that will depend on the separation of duties between the state and the local jurisdictions and the manner in which each state or local jurisdiction handles particular aspects of the election process.

Risks and threats
&&&&&&&&&&&&&&&&&

While EMSs are typically dedicated software that carries its own risks, that software generally runs on COTS software and hardware that operate in a networked environment. Many risks and threats associated with EMSs are similar to those of other systems running on COTS IT hardware and software, and include:

* Network connections with other internal systems, some of which may be owned or operated by other organizations or authorities,
* Security weaknesses in the underlying COTS products, whether hardware or software,
* Security weaknesses in the dedicated components, whether hardware or software,
* Errors in properly managing authentication and access control for authorized users,
* Difficulty associated with finding, and rolling back, improper changes found after the fact, and
* Infrastructure- and process-related issues associated with backup and auditing.

Significant consequences may result from successful attacks on an EMS. These potential consequences include the inability to properly control election processes and systems or, depending on the functions of the EMS, incorrect assignment of ballots to their respective precincts or other errors. Furthermore, successful manipulation of an EMS could result in cascading effects on other devices that are programmed from the EMS, potentially including voting machines and vote tabulation.

To help manage these risks, most election offices do not have network connections to their EMS, and rarely have internet connections. Instead, they keep the EMS isolated as a standalone machine or on a separate network that has no internet connection and is solely dedicated to the functioning of the EMS. Data transfers to and from the EMS are conducted with removable media only. This is an indirect connection and presents a particular set of risks to mitigate.

How these components connect
&&&&&&&&&&&&&&&&&&&&&&&&&&&&

The diversity of functions delivered by an EMS makes it difficult to generalize the level of connectedness of any given system, but most will have at least some aspects of a network connected system. A host of factors impact connectedness, such as whether a state or local EMS is network connected, communications with the EMS leverages connections such as a Secure File Transfer Protocol (SFTP), or all data is transferred through removable media. 

.. table:: Connection Types for Election Management Systems
   :widths: auto

   ==================================  =============================================================================
   Connectedness                       System Type and Additional Information
   ==================================  =============================================================================
   Network Connected                   Unless known definitively to have no network capabilities, treat an EMS as network connected.
   Indirectly Connected                If known definitively to have no network capabilities, treat an EMS as indirectly connected.
   Not Connected                       Not applicable.
   Additinal Transmission-based Risks  Not applicable.
   ==================================  =============================================================================

Vote capture
************

Vote capture devices are the means by which actual votes are cast and recorded. Approaches vary greatly both across and within jurisdictions. Any given jurisdiction, and even a single polling place, is likely to have multiple methods for vote capture to accommodate both administrative decisions and different needs of voters.

For instance, on election day, a polling place may give voters the choice of electronic ballot marking devices or paper ballots. Additionally, voters with language needs or voters with disabilities may necessitate the use of additional components or a separate device.

Because of this diversity in vote capture approaches, providing specific recommendations around vote capture security is a detailed task. The EAC, in coordination with other federal partners, state and local governments, vendors, and others in the elections community, maintain standards and a certification program for vote capture devices. We will not try to replicate or alter those recommendations here, but we will provide a set of threats, risks, and categorizations to help guide officials toward best practices for vote capture devices.

Vote capture devices are often top of mind when thinking of election security-—and for good reason. Vote capture devices are where democracy happens: the voices of the people are heard via the ballots they cast. But they are a single part of a larger ecosystem for which a holistic security approach is necessary. Much attention has been paid to vote capture devices, and these efforts should continue; ensuring the security of vote capture devices, like any aspect of security, is a continuous process.

The primary inputs to vote capture devices are the ballot definition file, which describes to the device how to display the ballot, an activation key (for some electronic machines), and the ballot itself for scanning of a paper ballot. The primary output is the cast vote record.

In cybersecurity, we often talk about non-repudiation: the inability to deny having taken an action. Our democracy is founded in the opposite principle: your ballot is secret; no one should be able to prove who or what you voted for or against in the voting booth. This presents an inherent difficulty in maintaining the security of the voting process. We intentionally create voter anonymity through a breakpoint between the fact that an individual voted and what votes they actually cast. We never want to enable the ability to look at a marked ballot and track it back to a specific voter.

Instead, we must carefully protect the integrity and secrecy of the vote cast through the capture process and into the process of tabulation. To do this, best practices call for applying a series of controls to mitigate the risk that a vote capture device is functioning improperly, to identify problems if they occur, and to recover without any loss of integrity.

Types of vote capture processes
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Vote capture generally occurs in one of six ways:

#. Voter marked and hand counted paper balloting. Ballots are typically pre-printed or printed on demand, given to voters who fill them out by hand, collected, and counted by hand. Hand counting represents a relatively small share of total votes. This category usually covers some mail-in ballots.
#. Voter marked paper balloting with scanning. Ballots are typically pre-printed or printed on demand, given to voters who fill them out by hand, and collected. Votes are tabulated by scanning the paper ballot with an optical or digital scanner, either individually or in batches. This category covers some mail-in ballots.
#. Electronic marking with paper ballot output. Rather than handing out a paper ballot, the voter is directed to a machine that displays the ballot. The voter casts votes, and the machine prints a marked ballot. These printed ballots are tabulated either individually or in batches. Votes are usually tabulated by scanning the paper ballot with an optical or digital scanner, though are sometimes counted by hand. The vote capture device does not store a record of the vote selections. This type of vote capture device is commonly referred to as a ballot marking device.
#. Electronic voting with paper record. The voter is directed to a machine that displays the ballot. The vote is captured on the machine and either transmitted digitally to a central machine for tabulation, or removable media is extracted from the machine at a later time to transmit a batch of captured votes. At the time the vote is captured, the machine creates a printed record of the vote selections that the voter can verify. That record remains with the machine. This type of vote capture device is commonly referred to as a direct record electronic (DRE) device with voter verifiable paper audit trail.
#. Electronic voting with no paper record. The same as electronic voting with paper record, but the machine does not print a record of the captured vote. Captured votes are only maintained digitally, typically in multiple physical locations on the device and, sometimes, on a centrally managed device at the polling location. This type of vote capture device is commonly referred to as a DRE device.
#. Electronic receipt and delivery of ballots conducted remotely. The majority of ballots received by voters using
this method are voters covered by the Uniformed and Overseas Citizens Absentee Voting Act (:term:UOCAVA). Though most UOCAVA votes involve paper ballots, there is a sub-set of this population that submits their marked ballot in a digitally-connected method such as email or fax. Once received digitally, the voter’s vote selections are transcribed so that the vote selections are integrated into the vote tabulation and results reporting systems; these systems do not have network connections to the voting system. Voting methods commonly called internet voting or mobile voting fall under this process.

Risks and threats
&&&&&&&&&&&&&&&&&

The consequences of a successful attack in a vote capture device are significant: the intentions of a voter are not properly reflected in the election results. The vast majority of vote capture devices are not network connected systems. This helps limit the attack paths and therefore the risks to which they are subject—in cybersecurity parlance, a non-networked approach substantially reduces the attack surface. Therefore, to change a large number of votes typically requires access to the vote capture machine hardware or software, or the ability to introduce errors through the devices that program the vote capture device or download results from the vote capture device. Moreover, most vote capture devices are tested and certified against criteria defined by the EAC, a state or local entity, or both, though evolving threats can change the risk profile of a device even if it has previously been certified.

The last type of vote capture described above, *'electronic receipt and delivery of ballots conducted remotely'* can take on a large number of flavors. In terms of cybersecurity-related risks, for activities like emailing marked ballots, election officials must consider especially risks involved in the transmission of the ballot. If the transmission of the marked ballot is done via digital means, it is subject to the risks of that transmission mode. 

Regardless of approach, risks exist, and they mostly stem from the transfer of data to or from vote capture machines. Specifically, they include:

* If ever networked, risks associated with established (whether persistent or intermittent) network connectivity,
* Risks associated with the corruption of removable media or temporary physical connections to systems that are networked,
* Security weaknesses in the underlying COTS products, whether hardware or software,
* Security weaknesses in proprietary products, whether hardware or software,
* Errors in properly managing authentication and access control for authorized users, and
* Difficulty associated with finding, and rolling back, improper changes found after the fact, especially in the context of ballot secrecy.

How these components connect
&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Each type of vote capture process should have risks evaluated individually based on its type of connectivity. Based on the type of connectivity for a given implementation, Part 3 provides mitigations for these risks.
Network Connected
If a vote capture machine transmits data for any reason—or even if the functionality is enabled regardless of whether it is used—it should be considered network connected.
Although many jurisdictions program the vote capture devices with the ballot definition using indirectly connected methods, some use methods to load the ballot definition files to the vote capture device by transmitting the data over a closed-local area network.
Also, many central count scanners, used for Voter marked paper balloting with scanning in batches (usually vote by mail ballots) are similarly networked on a closed-LAN.
Some electronic vote capture machines also directly transmit data for election night reporting.

.. table:: Connection Types for Vote Capture
   :widths: auto

   ==================================  =============================================================================
   Connectedness                       System Type and Additional Information
   ==================================  =============================================================================
   Network Connected                   Unless known definitively to have no network capabilities, treat an EMS as network connected.
   Indirectly Connected                If known definitively to have no network capabilities, treat an EMS as indirectly connected.
   Not Connected                       Not applicable.
   Additinal Transmission-based Risks  Not applicable.
   ==================================  =============================================================================

Indirectly Connected
1) Voter marked paper balloting with scanning. Paper ballots do not include an electronic component. While scanners are not typically network connected devices, they must be programmed to understand the ballot format and must transmit captured vote data to another, usually network connected, device.
2) Electronic voting with paper ballot output. In addition to the role of
the scanners, the vote capture machines are typically not network connected, but must be programmed to display the ballot and print the ballot in the correct format.
4) Electronic voting with paper record. The vote capture machines are typically not network connected but must be programmed to understand the ballot format and must transmit captured vote data to another, usually network connected, device.
5) Electronic voting with no paper record. The vote capture machines
are typically not network connected but must be programmed to understand the ballot format and must transmit captured vote data to another, usually network connected, device.
note: If a vote capture machine transmits data for any reason—or even if the functionality is enabled regardless of whether it is used—it should be considered network connected.
Not connected, out of scope
1) Voter marked and hand counted paper balloting. Out of scope in this handbook as the vote capture process does not include a digital component.
Additional transmission-based risks
6) Electronic voting conducted remotely. These methods vary greatly and must be addressed on a case-by-case basis. At minimum, when web-based, email, or fax transmission is used in either direction, it leverages a digital component and should incorporate the relevant transmission-based mitigations in Part 3. Aspects definitively executed without a digital component are not connected, out of scope.

Vote tabulation
In its broadest definition, vote tabulation is any aggregation or summation of votes. Vote tabulation is the aggregation of votes (e.g., cast vote records and vote summaries) for the purpose of generating totals and results report files. For the purposes of this handbook, this section on vote tabulation is considered separately from both the EMS of which tabulation is usually
a part, and vote capture machines that also tabulate (or aggregate). Vote tabulation in this handbook is focused on tabulation occurring across precincts, counties, etc., and covers both official and unofficial vote tabulation.
Risks and threats
Similar to vote capture devices, attacks on vote tabulation would seek to alter the counting of cast votes. This impact would be felt through the determination of the election outcome as well as the potential for confusion if initially reported outcomes did not agree with later certified results.
Vote tabulation typically involves either dedicated software or COTS software running on COTS hardware and operating systems, though some dedicated hardware is also in use. Vote capture devices most often transmit the vote data (e.g., results, cast vote records) to the vote tabulation system using removable media, though sometimes that data is transmitted across a network. Vote data is most often transferred across jurisdictions and to the state through uploads via direct connections such as a virtual private network, local network connections, faxes, or even phone calls.
The primary risks to vote tabulation are similar to those of other COTS- based systems: a compromise of the integrity or availability of aggregated votes totals could reduce confidence in an election, if not alter the outcome. Though the vote data is likely loaded to these systems via removable
media, most risks stem from vulnerabilities in these networked systems themselves. Such risks and threats include:
• Network connections with other internal systems, some of which may be owned or operated by other organizations or authorities,

• Security weaknesses in the underlying COTS products, whether hardware or software,
• Security weaknesses in proprietary products, whether hardware or software,
• Errors in properly managing authentication and access control for authorized users,
• Lack of confidentiality and integrity protection for transmitted results,
• Difficulty associated with finding, and rolling back, improper changes found after the fact, and
• Infrastructure- and process-related issues associated with backup and auditing.
These primary risks must be managed to ensure proper management of vote tabulation systems. Because they are risks and threats shared among users of COTS products, there is a well-established set of controls to mitigate risk and thwart threats.
How these components connect
Depending on the implementation, these systems should be considered network connected or indirectly connected. They may interface with the internet, and, even if they do not, almost certainly interface with a system that is connected to a network. Based on the type of connectivity for a given implementation, Part 3 provides mitigations for these risks.
Network Connected
In some cases, vote tabulation equipment will be network connected, whether through a wired or wireless connection.
Indirectly Connected
If vote tabulation equipment is not network connected, it is indirectly connected through removable media.

Not connected, out of scope
N/A
Additional transmission-based risks
N/A
Election results reporting and publishing
After votes are tabulated, results must be communicated both internally and to the public. In any given state, this can take many forms, but, in most cases, the basic process goal remains: getting results as quickly and accurately as possible. This section focuses on election night reporting, which involves unofficial results.
The inputs to election results reporting and publishing tabulated votes as described in the previous section. The systems used for reporting and publishing are likely networked, and, in many cases, have public facing websites.
The outputs are the unofficial election results, typically published on a website, often in multiple formats such as extensible markup language (XML), hypertext markup language (HTML), portable document format (PDF), and comma-separated values (CSV). There is likely a direct and persistent network connection between the published site and the internet, though the official record of the results may be kept on a system that is not persistently connected to the internet.

How these components connect
Depending on the approach to submitting tabulated votes, the reporting component may be network connected. The publishing component is almost certainly network connected, but may be indirectly connected, depending on the implementation. Based on the type of connectivity for a given implementation, Part 3 provides mitigations for these risks.
Network Connected
In some cases, election night reporting will be network connected, whether through a wired or wireless connection.
The publishing component of election night reporting is almost certainly network connected, whether through a wired or wireless connection.
Indirectly Connected
If the election night reporting process is not network connected, it is indirectly connected through removable media.
Not connected, out of scope
N/A
Additional transmission-based risks
N/A


