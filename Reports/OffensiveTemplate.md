# Red Team: Summary of Operations

## Table of Contents
- Exposed Services
- Critical Vulnerabilities
- Exploitation

### Exposed Services
_TODO: Fill out the information below._

Nmap scan results for each machine reveal the below services and OS details:

```bash
$ nmap ... # TODO: nmap -sV 192.168.1.110 
```

![](../Offensive/Service_Scan_Target_1.png)


This scan identifies the services below as potential points of entry:
- Target 1
  - Port 22/tcp SSH
  - Port 80/tcp Apache
  - Port 111/tcp Rpcbind
  - Port 139/tcp Netbios-ssn
  - Port 445/tcp Netbios-ssn

_TODO: Fill out the list below. Include severity, and CVE numbers, if possible._

The following vulnerabilities were identified on each target:
- Target 1
  - Wordpress User Enumertation 
  - Weak SSH Password
  - Plaintext Password for MySQL database
  - Unsalted Hashed Password in Wordpress Database

_TODO: Include vulnerability scan results to prove the identified vulnerabilities._

### Exploitation
_TODO: Fill out the details below. Include screenshots where possible._

The Red Team was able to penetrate `Target 1` and retrieve the following confidential data:
- Target 1
  - `flag1.txt`: flag1{b9bbcb33e11b80be759c4e844862482d}
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
  - `flag2.txt`: flag2{fcfd358dcdad9ab23faca6e9a36e581c}
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_