```
[*] Port scan All TCP Ports (all-tcp-ports) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/_full_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/xml/_full_tcp_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan wkhtmltoimage (tcp/5985/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png http://10.10.10.172:5985/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/tcp_5985_http_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Error: Failed to load http://10.10.10.172:5985/, with network status code 203 and http status code 404 - Error transferring http://10.10.10.172:5985/ - server replied: Not Found
[==============================>                             ] 50%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentNotFoundError


[*] Service scan Nmap Kerberos (tcp/88/kerberos-sec/nmap-kerberos) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 88 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp88/tcp_88_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp88/xml/tcp_88_kerberos_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap LDAP (tcp/389/ldap/nmap-ldap) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 389 --script="banner,(ldap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/tcp_389_ldap_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/xml/tcp_389_ldap_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap LDAP (tcp/3268/ldap/nmap-ldap) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 3268 --script="banner,(ldap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp3268/tcp_3268_ldap_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp3268/xml/tcp_3268_ldap_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap Kerberos (tcp/464/kpasswd5/nmap-kerberos) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 464 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp464/tcp_464_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp464/xml/tcp_464_kerberos_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/135/msrpc/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 135 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp135/tcp_135_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp135/xml/tcp_135_rpc_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap SMB (tcp/139/netbios-ssn/nmap-smb) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 139 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp139/tcp_139_smb_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp139/xml/tcp_139_smb_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap SMB (tcp/445/microsoft-ds/nmap-smb) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 445 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp445/tcp_445_smb_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp445/xml/tcp_445_smb_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/49667/msrpc/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 49667 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49667/tcp_49667_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49667/xml/tcp_49667_rpc_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/49674/msrpc/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 49674 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49674/tcp_49674_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49674/xml/tcp_49674_rpc_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/49676/msrpc/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 49676 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49676/tcp_49676_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49676/xml/tcp_49676_rpc_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/49693/msrpc/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 49693 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49693/tcp_49693_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49693/xml/tcp_49693_rpc_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap MSRPC (tcp/49747/msrpc/nmap-msrpc) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 49747 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49747/tcp_49747_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49747/xml/tcp_49747_rpc_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap DNS (tcp/53/domain/nmap-dns) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp53/tcp_53_dns_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp53/xml/tcp_53_dns_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap HTTP (tcp/5985/http/nmap-http) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -p 5985 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/tcp_5985_http_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/xml/tcp_5985_http_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Bug in http-security-headers: no string output.
Segmentation fault


[*] Port scan Top TCP Ports (top-tcp-ports) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/_quick_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/xml/_quick_tcp_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
adjust_timeouts2: packet supposedly had rtt of -179810 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -179810 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -205888 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -205888 microseconds.  Ignoring time.
Segmentation fault


[*] Port scan Top 100 UDP Ports (top-100-udp-ports) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/_top_100_udp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/xml/_top_100_udp_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
adjust_timeouts2: packet supposedly had rtt of -334280 microseconds.  Ignoring time.
adjust_timeouts2: packet supposedly had rtt of -334280 microseconds.  Ignoring time.
Segmentation fault


[*] Service scan Nmap Kerberos (udp/88/kerberos-sec/nmap-kerberos) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -sV -p 88 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp88/udp_88_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp88/xml/udp_88_kerberos_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap NTP (udp/123/ntp/nmap-ntp) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -sV -p 123 --script="banner,(ntp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp123/udp_123_ntp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp123/xml/udp_123_ntp_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault


[*] Service scan Nmap DNS (udp/53/domain/nmap-dns) ran a command which returned a non-zero exit code (139).
[-] Command: nmap -vv --reason -Pn -T4 -sU -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp53/udp_53_dns_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp53/xml/udp_53_dns_nmap.xml" 10.10.10.172
[-] Error Output:
Host discovery disabled (-Pn). All addresses will be marked 'up' and scan times may be slower.
Segmentation fault



```