```bash
nmap -vv --reason -Pn -T4 -sV -p 49153 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp49153/tcp_49153_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp49153/xml/tcp_49153_rpc_nmap.xml" 10.10.10.52
```

[/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp49153/tcp_49153_rpc_nmap.txt](file:///home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp49153/tcp_49153_rpc_nmap.txt):

```
# Nmap 7.92 scan initiated Sat Sep 24 16:48:29 2022 as: nmap -vv --reason -Pn -T4 -sV -p 49153 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp49153/tcp_49153_rpc_nmap.txt -oX /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp49153/xml/tcp_49153_rpc_nmap.xml 10.10.10.52
Nmap scan report for 10.10.10.52
Host is up, received user-set (0.014s latency).
Scanned at 2022-09-24 16:48:29 EDT for 75s

PORT      STATE SERVICE REASON          VERSION
49153/tcp open  msrpc   syn-ack ttl 127 Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Sat Sep 24 16:49:44 2022 -- 1 IP address (1 host up) scanned in 74.91 seconds

```
