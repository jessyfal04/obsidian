---
tags:
  - Room
---
*vulnerability research*
## Type of Vulnerabilities :

| Vulnerability               | Description / Exemples                                    |
| --------------------------- | --------------------------------------------------------- |
| Operating System            | OS, privilege escalation                                  |
| (Mis)Configuration-based    | Incorrectly configured website exposing customers details |
| Weak of Default Credentials | Default Passwords                                         |
| Application Logic           | Impersonate a user                                        |
| Human-Factor                | Trick human, phising                                      |
## Scoring :

#### **Common Vulnerability Scoring System (CVSS)**
1. Easiness to exploit
2. Existence of exploits
3. Interference the CIA triad
https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator

#### **Vulnerability Priority Rating (VPR)**
+ Organisation related
	+ Usage of the software or not
+ Not open source

## Vulnerability Databases

**Vulnerability** : Weakness in the design, implementation of a system or an application
**Exploit** : Action or behavior that utilizes a vulnerability on a system or an application
**Proof of Concept (PoC)** : Technique or tool to demonstrate the exploitation of the vulnerability

### NVD – National Vulnerability Database
https://nvd.nist.gov/vuln
**Common Vulnerabilities and Exposures (CVE)**
Format : `CVE-YEAR-IDNUMBER` (WannaCry : `CVE-2017-0144`)

### Exploit-DB
Can be used to get PoC

### **Version Disclosure**
Useful to find vulnerability
