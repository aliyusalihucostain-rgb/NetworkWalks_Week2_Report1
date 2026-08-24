# NetworkWalks_Week2_Report1
Kali Linux
<img width="663" height="568" alt="week 2 task 1" src="https://github.com/user-attachments/assets/922ad82f-1137-497e-a90d-91b69b6f1213" />
<img width="670" height="574" alt="week 2 task 2" src="https://github.com/user-attachments/assets/cf56d3db-8123-450f-ba31-f09c0280fb5c" />
<img width="673" height="610" alt="nslookup week 2" src="https://github.com/user-attachments/assets/1312a36b-6efd-4b20-bf85-1c29edb0db8e" />
<img width="659" height="607" alt="Curl week  2" src="https://github.com/user-attachments/assets/3dc23f93-7341-40d8-93ae-e2ecbd43594d" />
<img width="696" height="709" alt="dnsrecon week 2" src="https://github.com/user-attachments/assets/614c99dc-b7d1-4ad5-89d7-5bdd78a74efa" />
<img width="672" height="634" alt="wafwoof week 2" src="https://github.com/user-attachments/assets/10152640-2e9c-44fc-a722-da626c87bcfc" />

Zenmap
<img width="958" height="226" alt="task1" src="https://github.com/user-attachments/assets/a00dbb2b-a0b9-46ed-a606-748ee5ebd488" />
<img width="960" height="188" alt="task2" src="https://github.com/user-attachments/assets/89d2d069-5f12-4901-b69d-6a94c9e1cbce" />


Week 2 Report
Reconnaissance & Footprinting Techniques
Prepared By: Aliyu Salihu
Batch: Cybersecurity Professional — B082
Organization: Networkwalks Academy
Week: Week 2
Overview
This repository contains my Week 2 cybersecurity project for the Networkwalks Academy Cybersecurity Professional Program.
The project focused on Reconnaissance and Footprinting, an important phase of cybersecurity and penetration testing in which information about an authorized target is collected and analyzed before further security assessment.
The practical exercises involved the use of Kali Linux and Zenmap/Nmap, .
Ethical Notice: All activities documented in this report were conducted for educational purposes and against authorized targets or environments.

Learning Objectives
The main objectives of this week's practical exercises were to:
Understand the concepts of reconnaissance and footprinting.
Perform domain and DNS enumeration.
Obtain publicly available information about an authorized target.
Identify web technologies and server information.
Detect Web Application Firewall (WAF) protection.
Perform network host discovery and port scanning using Zenmap/Nmap.
Analyze reconnaissance results from a cybersecurity perspective.
Develop practical cybersecurity documentation and reporting skills.

Tools Used
Tool
Purpose
WHOIS
Domain registration and ownership information
WhatWeb
Web technology fingerprinting
nslookup
DNS resolution and lookup
curl
HTTP response and metadata analysis
WAFW00F
Web Application Firewall detection
dnsrecon
DNS enumeration
Nmap
Network discovery and port scanning
Zenmap
Graphical interface for Nmap


1. Kali Linux Multi-Tool Footprinting
The Kali Linux practical exercise involved using multiple reconnaissance tools to collect different categories of information about an authorized target.
Six reconnaissance tools were used during this exercise:
WHOIS
WhatWeb
nslookup
curl
WAFW00F
dnsrecon

WHOIS
WHOIS was used to obtain publicly available domain registration information associated with the authorized target.
The exercise focused on identifying information such as:
Registrar information
Domain registration details
Creation and expiry information
Name servers
Domain status information
The screenshot showing the WHOIS command and results is available in the Kali Linux folder.

WhatWeb
WhatWeb was used to perform web technology fingerprinting against the authorized target.
The purpose of the exercise was to identify technologies and components associated with the website.
Information that may be identified through the exercise includes:
Web server technology
Content Management System
JavaScript libraries
Web frameworks
Plugins
Other publicly detectable technologies
The corresponding evidence is provided in the Kali Linux folder.

nslookup
The nslookup utility was used to perform DNS resolution for the authorized target.
The exercise helped demonstrate how DNS information can be used to identify IP address information associated with a domain.
The command output is documented in the corresponding screenshot.



curl
The curl command was used to communicate with the authorized web server and inspect the HTTP response.
The exercise provided practical experience in examining information returned by a web server, including HTTP headers and other publicly exposed metadata.
The analysis focused on information such as:
HTTP response information
Server information
Redirects
Content-related headers
Publicly exposed metadata
The evidence is included in the Kali Linux folder.

WAFW00F
WAFW00F was used to determine whether a Web Application Firewall could be detected protecting the authorized web application.
A WAF can provide an additional security layer by filtering or monitoring potentially malicious web traffic
The result was recorded and analyzed as part of the reconnaissance process.

dnsrecon
dnsrecon was used to perform DNS enumeration against the authorized target.
The exercise demonstrated how DNS records can provide information about an organization's publicly exposed infrastructure.
The investigation considered records such as:
SOA records
NS records
A records
MX records
TXT records
SPF information
SRV records
The detailed command output is included in the evidence screenshots.

Kali Linux Reconnaissance Result
Using several tools rather than relying on a single reconnaissance technique provided a broader understanding of the authorized target.
WHOIS provided domain-registration information, WhatWeb provided technology fingerprinting, nslookup and dnsrecon provided DNS-related information, curl provided HTTP response information, and WAFW00F assisted in identifying possible web application security controls.
The combination of these results demonstrated the importance of correlating information obtained from multiple reconnaissance sources.
2. Network Scanning with Zenmap
Zenmap, the graphical interface for Nmap, was used to perform network reconnaissance in an authorized environment.
The practical exercise focused on host discovery and identifying network services exposed by the authorized target.

Quick Scan
A Quick Scan was performed to identify active hosts and accessible network services.
The actual Zenmap scan result is provided in the Zenmap directory.

Ping Scan
A Ping Scan was performed to determine whether the authorized target was reachable.
The scan focused on host discovery without conducting a detailed port scan.
Result
The result demonstrated how host discovery can be used as an initial stage of network reconnaissance.

Security Significance
Network scanning can provide valuable information about the services exposed by a system.
Open ports may indicate services that require appropriate security controls, access restrictions, monitoring, patching, and configuration.
For example, if Windows networking services such as SMB are exposed unnecessarily, they should be reviewed and appropriately restricted according to the organization's security requirements.
Challenges Faced
1. Different Reconnaissance Results
One of the challenges encountered during the practical exercises was that reconnaissance tools can produce different results depending on the target and information source being queried.
This demonstrated that reconnaissance results should not automatically be considered complete simply because one tool returned no information.
2. Combining Multiple Tools
Another challenge was understanding how to correlate information obtained from different tools.
Each tool provides a different perspective:
WHOIS focuses on domain registration information.
WhatWeb focuses on web technologies.
DNS tools reveal DNS-related information.
WAFW00F identifies possible WAF protection.
Nmap/Zenmap identifies hosts and network services.
Combining the results provided a more comprehensive understanding of the authorized environment.

3. Interpreting Results
Some command outputs contained technical information that required further interpretation.
The practical exercise improved my ability to distinguish between raw technical output and information that has actual security significance.

Lessons Learned
Through this Week 02 practical exercise, I learned that:
Reconnaissance is an important early phase of cybersecurity assessment.
No single reconnaissance tool provides a complete picture of a target.
DNS information can reveal useful infrastructure details.
Web fingerprinting can identify technologies that require security attention.
WAF detection can provide information about security controls protecting a web application.
OSINT can reveal relationships between domains, people, email addresses, websites, and other public entities.
Network scanning can identify active hosts and exposed services.
Open ports should be reviewed to determine whether the associated services are necessary and appropriately protected.
Reconnaissance information should be verified before being used for security decisions.
Cybersecurity reconnaissance must always be conducted within an authorized scope.
Conclusion
Week 02 provided practical experience with reconnaissance and footprinting techniques used in cybersecurity.
During the practical exercises, I worked with:
Kali Linux → WHOIS → WhatWeb → nslookup → curl → WAFW00F → dnsrecon → Zenmap/Nmap
The exercises demonstrated how different tools can be combined to collect, organize, and analyze information about an authorized target.
The practical work strengthened my understanding of:
OSINT
DNS enumeration
Domain footprinting
Web technology fingerprinting
HTTP metadata analysis
WAF detection
Network discovery
Port scanning
Security analysis and documentation
Most importantly, the exercise demonstrated that effective reconnaissance involves systematic collection, correlation, verification, and interpretation of information, rather than relying on a single tool.

References
Kali Linux — https://www.kali.org
Nmap — https://nmap.org
Zenmap — https://nmap.org/zenmap/
WAFW00F — https://github.com/EnableSecurity/wafw00f
dnsrecon — https://github.com/darkoperator/dnsrecon
Networkwalks Academy — https://networkwalks.com

Author
Aliyu Salihu
Cybersecurity Professional — B082
Networkwalks Academy
Week 02 — Reconnaissance & Footprinting Techniques
