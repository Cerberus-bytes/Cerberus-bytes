```bash
nmap -vv --reason -Pn -T4 -sV -p 464 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp464/tcp_464_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp464/xml/tcp_464_kerberos_nmap.xml" 10.10.10.52
```

[/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp464/tcp_464_kerberos_nmap.txt](file:///home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp464/tcp_464_kerberos_nmap.txt):

```
# Nmap 7.92 scan initiated Sat Sep 24 16:48:29 2022 as: nmap -vv --reason -Pn -T4 -sV -p 464 --script=banner,krb5-enum-users -oN /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp464/tcp_464_kerberos_nmap.txt -oX /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp464/xml/tcp_464_kerberos_nmap.xml 10.10.10.52
Nmap scan report for 10.10.10.52
Host is up, received user-set (0.014s latency).
Scanned at 2022-09-24 16:48:29 EDT for 20s

PORT    STATE SERVICE   REASON          VERSION
464/tcp open  kpasswd5? syn-ack ttl 127

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Sat Sep 24 16:48:49 2022 -- 1 IP address (1 host up) scanned in 19.90 seconds

```