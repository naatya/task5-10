# task5-10
Malware Types &amp; Behavior Analysis

**Task Summary**

This project involved a comprehensive study of malware types, their lifecycles, and practical analysis using industry-standard tools like VirusTotal within a Kali Linux environment. The goal was to understand how threats operate and how to defend against them.

Step-by-Step Technical Activities

**1. Malware Categorization**
Researched and identified the core differences between major malware families:

**Virus:** Programs that require human action to spread and infect other files.

**Worms:** Self-replicating malware that spreads across networks without human intervention.

**Trojans:** Malicious software disguised as legitimate programs to gain unauthorized access.

**Ransomware:** Malware that encrypts user data and demands payment for the decryption key.

**2. Hash-Based Analysis (Static Analysis)**
Selected known malware samples and extracted their unique identifiers (MD5/SHA-256 hashes).

Uploaded these hashes to VirusTotal to leverage 90+ antivirus engines for detection.

**Tools Used**: sha256sum, md5sum in the Kali Terminal.

**3. Detection Report Interpretation**
Analyzed VirusTotal reports to understand detection ratios.

Studied the "Details" tab to identify file headers, entropy, and signature timestamps.

Reviewed the "Community" tab for expert insights and sandbox execution notes.

**4. Behavioral Observation**
Observed Indicators of Compromise (IoCs) such as:

Registry key modifications.

Network connections to suspicious C2 (Command & Control) IPs.

File system changes (dropping .dll or .tmp files).

**5. Understanding the Malware Lifecycle**
Mapped the progression of an attack through the following stages:

**Delivery**: Email phishing, malicious links, or infected USBs.

**Exploitation**: Triggering a vulnerability in the target system.

**Installation**: Establishing a foothold (persistence).

**Execution**: Carrying out the intended malicious activity (the "Payload").

**6. Propagation & Spreading Mechanisms**
Explored how malware moves laterally:

Exploiting network protocols (SMB, RDP).

Social engineering (tricking users).

Drive-by downloads from compromised websites.

**7. Prevention & Mitigation Strategies**
Identified key defense-in-depth methods:

**Endpoint Protection:** Using EDR and updated Antivirus.

**Network Security:** Implementing firewalls and IDS/IPS.

**User Awareness**: Training against phishing and social engineering.

**Backup Policy**: Maintaining offline backups to mitigate Ransomware impact.

**Key Findings & Conclusion**
The analysis demonstrated that while many threats are detected by signature-based scanning (0/92 results), sophisticated malware often uses obfuscation to hide. A combination of static analysis (hashes) and behavioral monitoring is essential for modern cybersecurity defense.
