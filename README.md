# Tsang-Pak-Ho-COMP3000HK
COMP3000HK Computing Project

**Project Title**
Comparing Signature-Based and Behavioral Log Analysis for Detecting Web Server Memory Attacks

**Keywords**
Zero-day attack, log analysis, behavioral detection, signature detection, PHP server, memory exhaustion   

**Project Vision**
For my project, I want to build a Python tool that looks at web server logs to find memory-exhaustion attacks. I am focusing on a recent real-world problem (the PHP CVE-2026-109618 vulnerability). I will set up a test server, send normal traffic and attack traffic to it, and see which detection method works better: looking for known attack signatures, or looking for unusual behavior. My goal is to find out if the behavioral method is actually worth the extra processing time it takes, which would help security teams make better decisions.   

**Literature Review**
Before I start coding, I will research three main areas. First, I need to understand how memory exhaustion attacks work, especially the recent PHP issue, so I know what I am trying to detect. Second, I will look into how traditional Web Application Firewalls (WAFs) use signature rules to block bad traffic and why they usually fail when a brand-new attack comes out. Third, I will read up on behavioral anomaly detection—basically how systems learn what "normal" traffic looks like so they can spot weird patterns. I plan to use reports from cybersecurity agencies like CISA and academic papers on network intrusion detection to guide my work.   

**Risk Assessment**
The primary risk is not having the exact hacker code for the PHP attack since it is brand new. But I don't need the real malware because I will just write a Python script that mimics the heavy network traffic hackers use to crash the server. As long as it crashes the memory, the logs will be useful. 
Another risk is not having enough "normal" background traffic to test against, which would mess up my false-positive results. To tackle this, I will write a separate Python script to constantly browse my test server to simulate real users. I will leave this running for a while to build a solid baseline of normal logs.

**Gantt Chart / Project Plan**
Please see the [Project_Gantt_Chart_Updated.xlsx](https://github.com/user-attachments/files/34584312/Project_Gantt_Chart_Updated.xlsx)
