```bash
nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/_quick_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/xml/_quick_tcp_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/_full_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/xml/_full_tcp_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/_top_100_udp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/xml/_top_100_udp_nmap.xml" 10.10.10.172

dig -p 53 -x 10.10.10.172 @10.10.10.172

dig AXFR -p 53 @10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp53/tcp_53_dns_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp53/xml/tcp_53_dns_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 88 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp88/tcp_88_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp88/xml/tcp_88_kerberos_nmap.xml" 10.10.10.172

impacket-getArch -target 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 135 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp135/tcp_135_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp135/xml/tcp_135_rpc_nmap.xml" 10.10.10.172

impacket-rpcdump -port 135 10.10.10.172

enum4linux -a -M -l -d 10.10.10.172 2>&1

nbtscan -rvh 10.10.10.172 2>&1

nmap -vv --reason -Pn -T4 -sV -p 139 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp139/tcp_139_smb_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp139/xml/tcp_139_smb_nmap.xml" 10.10.10.172

smbclient -L //10.10.10.172 -N -I 10.10.10.172 2>&1

smbmap -H 10.10.10.172 -P 139 2>&1

nmap -vv --reason -Pn -T4 -sV -p 389 --script="banner,(ldap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/tcp_389_ldap_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/xml/tcp_389_ldap_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 445 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp445/tcp_445_smb_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp445/xml/tcp_445_smb_nmap.xml" 10.10.10.172

smbmap -H 10.10.10.172 -P 445 2>&1

nmap -vv --reason -Pn -T4 -sV -p 464 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp464/tcp_464_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp464/xml/tcp_464_kerberos_nmap.xml" 10.10.10.172

impacket-rpcdump -port 593 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 3268 --script="banner,(ldap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp3268/tcp_3268_ldap_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp3268/xml/tcp_3268_ldap_nmap.xml" 10.10.10.172

feroxbuster -u http://10.10.10.172:5985/ -t 10 -w /root/.config/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -o "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/tcp_5985_http_feroxbuster_dirbuster.txt"

curl -sSikf http://10.10.10.172:5985/.well-known/security.txt

curl -sSikf http://10.10.10.172:5985/robots.txt

curl -sSik http://10.10.10.172:5985/

nmap -vv --reason -Pn -T4 -sV -p 5985 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/tcp_5985_http_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/xml/tcp_5985_http_nmap.xml" 10.10.10.172

whatweb --color=never --no-errors -a 3 -v http://10.10.10.172:5985 2>&1

wkhtmltoimage --format png http://10.10.10.172:5985/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp5985/tcp_5985_http_screenshot.png

nmap -vv --reason -Pn -T4 -sV -p 49667 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49667/tcp_49667_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49667/xml/tcp_49667_rpc_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 49674 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49674/tcp_49674_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49674/xml/tcp_49674_rpc_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 49676 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49676/tcp_49676_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49676/xml/tcp_49676_rpc_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 49693 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49693/tcp_49693_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49693/xml/tcp_49693_rpc_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sV -p 49747 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49747/tcp_49747_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp49747/xml/tcp_49747_rpc_nmap.xml" 10.10.10.172

smbmap -u null -p "" -H 10.10.10.172 -P 445 2>&1

smbmap -H 10.10.10.172 -P 445 -R 2>&1

smbmap -u null -p "" -H 10.10.10.172 -P 445 -R 2>&1

smbmap -H 10.10.10.172 -P 445 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.10.172 -P 445 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.10.172 -P 139 2>&1

smbmap -H 10.10.10.172 -P 139 -R 2>&1

smbmap -u null -p "" -H 10.10.10.172 -P 139 -R 2>&1

smbmap -H 10.10.10.172 -P 139 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.10.172 -P 139 -x "ipconfig /all" 2>&1

dig -p 53 -x 10.10.10.172 @10.10.10.172

dig AXFR -p 53 @10.10.10.172

nmap -vv --reason -Pn -T4 -sU -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp53/udp_53_dns_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp53/xml/udp_53_dns_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sU -sV -p 88 --script="banner,krb5-enum-users" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp88/udp_88_kerberos_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp88/xml/udp_88_kerberos_nmap.xml" 10.10.10.172

nmap -vv --reason -Pn -T4 -sU -sV -p 123 --script="banner,(ntp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp123/udp_123_ntp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/udp123/xml/udp_123_ntp_nmap.xml" 10.10.10.172


```