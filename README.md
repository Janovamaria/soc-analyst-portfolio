Case 1: RDP Brute Force Detected (Event ID 234)

Alert Type: Network / Brute Force | Target Port: 3389 (RDP)

Summary:
Investigated an alert for repeated RDP login attempts from external source IP 218.92.0.56 targeting port 3389.

Investigation Steps:


Confirmed 218.92.0.56 as a public/external IP (not in any private IP range)
Reviewed connection attempts for volume and pattern consistent with automated brute-force behavior
Logged artifacts (source IP, targeted port) for the case record
[Fill in: was the connection blocked or did it succeed? Any specific username targeted?]


Conclusion: True Positive — external attacker attempting unauthorized RDP access via brute force. Recommended blocking the source IP at the firewall and reviewing whether RDP needs to be exposed to the internet at all.


Skills Demonstrated


SOC alert triage and case management workflow
Log analysis and IOC (Indicator of Compromise) identification
Distinguishing internal vs. external IP addresses
Mapping attacker behavior to MITRE ATT&CK techniques
Evidence-based incident classification (True Positive / False Positive)
Incident documentation and reporting


Tools Used

LetsDefend (SIEM/SOC simulation), Log Management, Case Management, Endpoint Security modules
