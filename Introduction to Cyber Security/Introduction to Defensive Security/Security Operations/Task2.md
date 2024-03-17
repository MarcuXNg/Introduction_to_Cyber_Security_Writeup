### Data Sources
Data sources that are used to monitor the network for signs of intrusions and to detect any malicious behaviour:
- `Server logs`: There are many types of servers on a network, such as a mail server, web server, and domain controller on MS Windows networks. Logs contain information about various activities, such as successful and failed login attempts, among many others. There is a trove of information that can be found in the server logs.

- `DNS activity`: DNS stands for Domain Name System, and it is the protocol responsible for converting a domain name, such as `tryhackme.com`, to an IP address, such as 10.3.13.37, among other domain name related queries (In practice, if someone tries to browse `tryhackme.com`, the DNS server has to resolve it and can log the DNS query to monitoring. The SOC can gather information about domain names that internal systems are trying to communicate with by merely inspecting DNS queries).

- `Firewall logs`: A firewall is a device that controls network packets entering and leaving the network mainly by letting them through or blocking them. Consequently, firewall logs can reveal much information about what packets passed or tried to pass through the firewall.

- `DHCP logs`: DHCP stands for Dynamic Host Configuration Protocol, and it is responsible for assigning an IP address to the systems that try to connect to a network. Know that DHCP has automatically provided your device with the network settings whenever you can join a network without manual configuration. Inspecting DHCP transactions => learn about the devices that joined the network.

- Other: `Security Information` and `Event Management (SIEM) system` (The SIEM aggregates the data from the different sources so that the SOC can efficiently correlate the data and respond to attacks.)

### SOC Services
- SOC services include `reactive` and `proactive services` in addition to other services.
    + `Reactive` services refer to the tasks initiated after detecting an intrusion or a malicious event":
        * `Monitor security posture`: The primary role of the SOC, includes monitoring the network and computers for security alerts and notifications and responding to them as the need dictates.

        * `Vulnerability management`: Finding vulnerabilities in the company systems and patching (fixing) them. The SOC can assist with this task but not necessarily execute it.

        * `Malware analysis`: The SOC might recover malicious programs that reached the network. The SOC can do basic analysis by executing it in a controlled environment. However, more advanced analysis requires sending it to a dedicated team.

        * `Intrusion detection`: An intrusion detection system (IDS) is used to detect and log intrusions and suspicious packets. The SOC’s job is to maintain such a system, monitor its alerts, and go through its logs as the need dictates.

        * `Reporting`: It is essential to report incidents and alarms. Reporting is necessary to ensure a smooth workflow and to support compliance requirements.

    + `Proactive` services refer to the tasks handled by the SOC without any indicator of an intrusion:

        * `Network security monitoring (NSM)`: This focuses on monitoring the network data and analyzing the traffic to detect signs of intrusions.

        * `Threat hunting`: The SOC assumes an intrusion has already taken place and begins its hunt to see if they can confirm this assumption.
        
        * `Threat Intelligence`: Threat intelligence focuses on learning about potential adversaries and their tactics and techniques to improve the company’s defences. The purpose would be to establish a threat-informed defence.
