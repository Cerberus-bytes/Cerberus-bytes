```bash
nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/_top_100_udp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/xml/_top_100_udp_nmap.xml" 10.10.10.52
```

[/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/_top_100_udp_nmap.txt](file:///home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.92 scan initiated Sat Sep 24 16:47:04 2022 as: nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/_top_100_udp_nmap.txt -oX /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/xml/_top_100_udp_nmap.xml 10.10.10.52
Nmap scan report for 10.10.10.52
Host is up, received user-set (0.025s latency).
Scanned at 2022-09-24 16:47:05 EDT for 147s
Not shown: 96 closed udp ports (port-unreach)
PORT     STATE         SERVICE      REASON       VERSION
88/udp   open          kerberos-sec udp-response Microsoft Windows Kerberos (server time: 2022-09-24 20:47:13Z)
137/udp  open|filtered netbios-ns   no-response
138/udp  open|filtered netbios-dgm  no-response
4500/udp open|filtered nat-t-ike    no-response
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.92%E=4%D=9/24%OT=%CT=%CU=7%PV=Y%DS=2%DC=T%G=N%TM=632F6D5C%P=x86_64-pc-linux-gnu)
SEQ(CI=I%II=I)
T5(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
T6(R=Y%DF=Y%T=80%W=0%S=A%A=O%F=R%O=%RD=0%Q=)
T7(R=Y%DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)
IE(R=Y%DFI=N%T=80%CD=Z)

Network Distance: 2 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

TRACEROUTE (using port 998/udp)
HOP RTT      ADDRESS
1   27.57 ms 10.10.14.1
2   35.47 ms 10.10.10.52

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Sat Sep 24 16:49:32 2022 -- 1 IP address (1 host up) scanned in 147.98 seconds

```