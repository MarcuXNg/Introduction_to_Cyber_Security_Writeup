### Security Operations Center (SOC)

- a team of cyber security professionals that monitors the network and its systems to detect malicious cyber security events.

    + Vulnerabilities: 
        - Whenever a system vulnerability (weakness) is discovered, it is essential to fix it by installing a proper update or patch.
        - When a fix is not available, the necessary measures should be taken to prevent an attacker from exploiting it. 
        - Although remediating vulnerabilities is of vital interest to a SOC, it is not necessarily assigned to them.
    + Policy violations: 
        - We can think of a security policy as a set of rules required for the protection of the network and systems. 
        - For example, it might be a policy violation if users start uploading confidential company data to an online storage service.
    + Unauthorized activity: 
        - Consider the case where a user’s login name and password are stolen, and the attacker uses them to log into the network.
        - A SOC needs to detect such an event and block it as soon as possible before further damage is done.
    + Network intrusions:
        - No matter how good your security is, there is always a chance for an intrusion. An intrusion can occur when a user clicks on a malicious link or when an attacker exploits a public server. 
        - Either way, when an intrusion occurs, we must detect it as soon as possible to prevent further damage.

### Threat Intelligence

+ Intelligence refers to information you gather about actual and potential enemies.
+ A threat is any action that can disrupt or adversely affect a system
+ help the company better prepare against potential adversaries.
+ purpose to achieve a threat-informed defense

- Different companies have different adversaries. Based on the company (target), we can expect adversaries.

- Intelligence needs data
    + Data has to be collected, processed, and analyzed.
    + Data collection is done from local sources such as network logs and public sources such as forums
    + Processing of data aims to arrange them into a format suitable for analysis
    + The analysis phase seeks to find more information about the attackers and their motives; moreover, it aims to create a list of recommendations and actionable steps.

- Learning about your adversaries allows you to know their tactics, techniques, and procedures
-  As a result of threat intelligence
  + identify the threat actor (adversary), 
  + predict their activity, 
  + mitigate their attacks and prepare a response strategy.

### Digital Forensics

- Forensics is the application of science to investigate crimes and establish facts
- With the use and spread of digital systems, such as computers and smartphones, a new branch of forensics was born to investigate related crimes: computer forensics
- analyzing evidence of an attack and its perpetrators and other areas such as intellectual property theft, cyber espionage, and possession of unauthorized content

- Focus on different areas:
    - `File System`: Analyzing a digital forensics image (low-level copy) of a system’s storage reveals much information, such as installed programs, created files, partially overwritten files, and deleted files.
    - `System memory`: If the attacker is running their malicious program in memory without saving it to the disk, taking a forensic image (low-level copy) of the system memory is the best way to analyze its contents and learn about the attack.
    - `System logs`: Each client and server computer maintains different log files about what is happening. Log files provide plenty of information about what happened on a system. Some traces will be left even if the attacker tries to clear their traces.
    - `Network logs`: Logs of the network packets that have traversed a network would help answer more questions about whether an attack is occurring and what it entails.

### Incident Response

- An incident: usually refers to a data breach or cyber attack; however, in some cases, it can be something less critical, such as a misconfiguration, an intrusion attempt, or a policy violation.
- cyber attack: making our network or systems inaccessible, defacing (changing) the public website, and data breach (stealing company data)
- Incident response specifies the methodology that should be followed to handle such a case.
=> reduce damage and recover in the shortest time possible.
=> develop a plan ready for incident response.

[The four major phases of the incident response process]:
- `Preparation`: This requires a team trained and ready to handle incidents. Ideally, various measures are put in place to prevent incidents from happening in the first place.
- `Detection and Analysis`: The team has the necessary resources to detect any incident; moreover, it is essential to further analyze any detected incident to learn about its severity.
- `Containment, Eradication, and Recovery`: Once an incident is detected, it is crucial to stop it from affecting other systems, eliminate it, and recover the affected systems. For instance, when we notice that a system is infected with a computer virus, we would like to stop (contain) the virus from spreading to other systems, clean (eradicate) the virus, and ensure proper system recovery.
- `Post-Incident Activity`: After successful recovery, a report is produced, and the learned lesson is shared to prevent similar future incidents.

### Malware Analysis

- Malware stands for malicious software
- Software refers to programs, documents, and files that you can save on a disk or send over the network

+ Virus: a piece of code (part of a program) that attaches itself to a program. It is designed to spread from one computer to another; moreover, it works by altering, overwriting, and deleting files once it infects a computer. The result ranges from the computer becoming slow to unusable.
+ Trojan Horse: a program that shows one desirable function but hides a malicious function underneath. (can give attackers full control)
+ Ransomware: a malicious program that encrypts the user’s files. Encryption makes the files unreadable without knowing the encryption password. The attacker offers the user the encryption password if the user is willing to pay a “ransom.”

=> Static analysis works by inspecting the malicious program without running it. Usually, this requires solid knowledge of assembly language (processor’s instruction set, i.e., computer’s fundamental instructions).
=> Dynamic analysis works by running the malware in a controlled environment and monitoring its activities. It lets you observe how the malware behaves when running.
