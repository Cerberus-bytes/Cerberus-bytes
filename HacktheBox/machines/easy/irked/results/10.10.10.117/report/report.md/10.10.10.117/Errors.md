```
[*] Port scan Top TCP Ports (top-tcp-ports) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/_quick_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/xml/_quick_tcp_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
adjust_timeouts2: packet supposedly had rtt of -389766 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -389766 microseconds.  Ignoring time.
Segmentation fault


[*] Service scan showmount (tcp/111/rpcbind/showmount) ran a command which returned a non-zero exit code (1).
[-] Command: showmount -e 10.10.10.117 2>&1
[-] Error Output:


[*] Port scan All TCP Ports (all-tcp-ports) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/_full_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/xml/_full_tcp_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
adjust_timeouts2: packet supposedly had rtt of -537397 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -537397 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -538943 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -538943 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -94315 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -94315 microseconds.  Ignoring time.
Segmentation fault


[*] Service scan Nmap SSH (tcp/22/ssh/nmap-ssh) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 22 --script="banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp22/tcp_22_ssh_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp22/xml/tcp_22_ssh_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/111/rpcbind/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 111 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/tcp_111_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/xml/tcp_111_rpc_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap NFS (tcp/111/rpcbind/nmap-nfs) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 111 --script="banner,(rpcinfo or nfs*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/tcp_111_nfs_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/xml/tcp_111_nfs_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap HTTP (tcp/80/http/nmap-http) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 80 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp80/tcp_80_http_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp80/xml/tcp_80_http_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Bug in http-security-headers: no string output.
Segmentation fault


[*] Service scan Nmap IRC (tcp/6697/irc/nmap-irc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV --script irc-botnet-channels,irc-info,irc-unrealircd-backdoor -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp6697/tcp_6697_irc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp6697/xml/tcp_6697_irc_nmap.xml" -p 6697 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap IRC (tcp/8067/irc/nmap-irc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV --script irc-botnet-channels,irc-info,irc-unrealircd-backdoor -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp8067/tcp_8067_irc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp8067/xml/tcp_8067_irc_nmap.xml" -p 8067 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap IRC (tcp/65534/irc/nmap-irc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV --script irc-botnet-channels,irc-info,irc-unrealircd-backdoor -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp65534/tcp_65534_irc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp65534/xml/tcp_65534_irc_nmap.xml" -p 65534 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Port scan Top 100 UDP Ports (top-100-udp-ports) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/_top_100_udp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/xml/_top_100_udp_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan showmount (udp/111/rpcbind/showmount) ran a command which returned a non-zero exit code (1).
[-] Command: showmount -e 10.10.10.117 2>&1
[-] Error Output:


[*] Service scan Nmap MSRPC (udp/111/rpcbind/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -sV -p 111 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/udp_111_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/xml/udp_111_rpc_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap NFS (udp/111/rpcbind/nmap-nfs) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -sV -p 111 --script="banner,(rpcinfo or nfs*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/udp_111_nfs_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/xml/udp_111_nfs_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap Multicast DNS (udp/5353/mdns/nmap-multicast-dns) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -sV -p 5353 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp5353/udp_5353_multicastdns_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp5353/xml/udp_5353_multicastdns_nmap.xml" 10.10.10.117
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault



```