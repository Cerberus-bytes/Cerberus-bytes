```bash
nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/_quick_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/xml/_quick_tcp_nmap.xml" 10.10.10.117

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/_full_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/xml/_full_tcp_nmap.xml" 10.10.10.117

nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/_top_100_udp_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/xml/_top_100_udp_nmap.xml" 10.10.10.117

nmap -vv --reason -Pn -T4 -sV -p 22 --script="banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp22/tcp_22_ssh_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp22/xml/tcp_22_ssh_nmap.xml" 10.10.10.117

feroxbuster -u http://10.10.10.117:80/ -t 10 -w /root/.config/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -o "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp80/tcp_80_http_feroxbuster_dirbuster.txt"

curl -sSikf http://10.10.10.117:80/.well-known/security.txt

curl -sSikf http://10.10.10.117:80/robots.txt

curl -sSik http://10.10.10.117:80/

nmap -vv --reason -Pn -T4 -sV -p 80 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp80/tcp_80_http_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp80/xml/tcp_80_http_nmap.xml" 10.10.10.117

whatweb --color=never --no-errors -a 3 -v http://10.10.10.117:80 2>&1

wkhtmltoimage --format png http://10.10.10.117:80/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp80/tcp_80_http_screenshot.png

nmap -vv --reason -Pn -T4 -sV -p 111 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/tcp_111_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/xml/tcp_111_rpc_nmap.xml" 10.10.10.117

nmap -vv --reason -Pn -T4 -sV -p 111 --script="banner,(rpcinfo or nfs*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/tcp_111_nfs_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp111/xml/tcp_111_nfs_nmap.xml" 10.10.10.117

showmount -e 10.10.10.117 2>&1

nmap -vv --reason -Pn -T4 -sV --script irc-botnet-channels,irc-info,irc-unrealircd-backdoor -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp6697/tcp_6697_irc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp6697/xml/tcp_6697_irc_nmap.xml" -p 6697 10.10.10.117

nmap -vv --reason -Pn -T4 -sV --script irc-botnet-channels,irc-info,irc-unrealircd-backdoor -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp8067/tcp_8067_irc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp8067/xml/tcp_8067_irc_nmap.xml" -p 8067 10.10.10.117

nmap -vv --reason -Pn -T4 -sV --script irc-botnet-channels,irc-info,irc-unrealircd-backdoor -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp65534/tcp_65534_irc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/tcp65534/xml/tcp_65534_irc_nmap.xml" -p 65534 10.10.10.117

nmap -vv --reason -Pn -T4 -sU -sV -p 111 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/udp_111_rpc_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/xml/udp_111_rpc_nmap.xml" 10.10.10.117

nmap -vv --reason -Pn -T4 -sU -sV -p 111 --script="banner,(rpcinfo or nfs*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/udp_111_nfs_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp111/xml/udp_111_nfs_nmap.xml" 10.10.10.117

showmount -e 10.10.10.117 2>&1

nmap -vv --reason -Pn -T4 -sU -sV -p 5353 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp5353/udp_5353_multicastdns_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/irked/results/10.10.10.117/scans/udp5353/xml/udp_5353_multicastdns_nmap.xml" 10.10.10.117


```