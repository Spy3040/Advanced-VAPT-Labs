Assessment Type: Internal VAPT (Lab Simulation)
Testing Approach: Black-box
Tools Used: Kali Linux, Metasploit, OpenVAS

# OpenVAS Vulnerability Findings Log

| Timestamp            | Target IP        | Vulnerability | PTES Phase     |
|----------------------|------------------|---------------|----------------|
| 2025-08-25 13:00:00  | 192.168.1.150    | Drupal RCE    | Exploitation   |

## Description
OpenVAS identified a critical remote code execution vulnerability affecting the web application hosted on the target system. This vulnerability could allow an attacker to execute arbitrary commands on the server.


# Exploitation Simulation

## Exploit Used
Metasploit module: exploit/linux/http/drupal_drupageddon

## Exploitation Phase
The identified Drupal RCE vulnerability was mapped to the exploitation phase of the PTES methodology. Successful exploitation of this vulnerability could allow attackers to gain remote command execution on the target server.

## Impact
If exploited, an attacker could gain full control over the affected system, install backdoors, access sensitive files, and potentially move laterally within the network.

# Remediation and Verification

## Recommended Remediation
- Apply the latest security patches and updates for Drupal
- Restrict access to administrative interfaces
- Implement Web Application Firewall (WAF) rules
- Perform regular vulnerability scans

## Verification
After applying the recommended fixes, a rescan should be conducted using OpenVAS to verify that the identified vulnerabilities have been successfully mitigated.

# Penetration Testing Report – Capstone Project

## Executive Summary
A vulnerability assessment and penetration testing (VAPT) engagement was conducted against a lab-based target system to evaluate its security posture. The assessment identified a critical remote code execution vulnerability within a web application component. If exploited, this vulnerability could result in complete system compromise.

## Findings
OpenVAS identified a Drupal remote code execution vulnerability on the target host (192.168.1.150). This vulnerability was mapped to the exploitation phase of the Penetration Testing Execution Standard (PTES). The flaw could allow attackers to execute arbitrary commands on the server with elevated privileges.

## Recommendations
It is recommended to apply the latest security patches, restrict access to administrative interfaces, and enforce secure configuration practices. Regular vulnerability scanning and timely patch management should be implemented to reduce future risk.

Overall, remediation of the identified issue will significantly improve the system’s resilience against common attack techniques.

# Management Briefing

The security assessment identified a critical weakness in the system that could allow attackers to gain full control of the server. If left unaddressed, this issue could result in data loss, service disruption, and reputational damage.

Applying security updates and following secure configuration practices will significantly reduce this risk. Regular security testing is recommended to ensure continued protection of critical systems.

