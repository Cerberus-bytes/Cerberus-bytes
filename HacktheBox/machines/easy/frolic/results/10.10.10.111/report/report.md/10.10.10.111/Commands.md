```bash
nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/_quick_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/xml/_quick_tcp_nmap.xml" 10.10.10.111

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/_full_tcp_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/xml/_full_tcp_nmap.xml" 10.10.10.111

nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/_top_100_udp_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/xml/_top_100_udp_nmap.xml" 10.10.10.111

nmap -vv --reason -Pn -T4 -sV -p 22 --script="banner,ssh2-enum-algos,ssh-hostkey,ssh-auth-methods" -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp22/tcp_22_ssh_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp22/xml/tcp_22_ssh_nmap.xml" 10.10.10.111

enum4linux -a -M -l -d 10.10.10.111 2>&1

nbtscan -rvh 10.10.10.111 2>&1

nmap -vv --reason -Pn -T4 -sV -p 139 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp139/tcp_139_smb_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp139/xml/tcp_139_smb_nmap.xml" 10.10.10.111

smbclient -L //10.10.10.111 -N -I 10.10.10.111 2>&1

smbmap -H 10.10.10.111 -P 139 2>&1

nmap -vv --reason -Pn -T4 -sV -p 445 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp445/tcp_445_smb_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp445/xml/tcp_445_smb_nmap.xml" 10.10.10.111

smbmap -H 10.10.10.111 -P 445 2>&1

feroxbuster -u http://10.10.10.111:9999/ -t 10 -w /root/.config/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -o "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp9999/tcp_9999_http_feroxbuster_dirbuster.txt"

curl -sSikf http://10.10.10.111:9999/.well-known/security.txt

curl -sSikf http://10.10.10.111:9999/robots.txt

curl -sSik http://10.10.10.111:9999/

nmap -vv --reason -Pn -T4 -sV -p 9999 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp9999/tcp_9999_http_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp9999/xml/tcp_9999_http_nmap.xml" 10.10.10.111

whatweb --color=never --no-errors -a 3 -v http://10.10.10.111:9999 2>&1

wkhtmltoimage --format png http://10.10.10.111:9999/ /home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp9999/tcp_9999_http_screenshot.png

smbmap -u null -p "" -H 10.10.10.111 -P 139 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 445 2>&1

smbmap -H 10.10.10.111 -P 139 -R 2>&1

smbmap -H 10.10.10.111 -P 445 -R 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 139 -R 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 445 -R 2>&1

smbmap -H 10.10.10.111 -P 445 -x "ipconfig /all" 2>&1

smbmap -H 10.10.10.111 -P 139 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 445 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 139 -x "ipconfig /all" 2>&1

feroxbuster -u http://10.10.10.111:1880/ -t 10 -w /root/.config/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -o "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp1880/tcp_1880_http_feroxbuster_dirbuster.txt"

curl -sSikf http://10.10.10.111:1880/.well-known/security.txt

curl -sSikf http://10.10.10.111:1880/robots.txt

curl -sSik http://10.10.10.111:1880/

nmap -vv --reason -Pn -T4 -sV -p 1880 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp1880/tcp_1880_http_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp1880/xml/tcp_1880_http_nmap.xml" 10.10.10.111

whatweb --color=never --no-errors -a 3 -v http://10.10.10.111:1880 2>&1

wkhtmltoimage --format png http://10.10.10.111:1880/ /home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp1880/tcp_1880_http_screenshot.png

nmap -vv --reason -Pn -T4 -sU -sV -p 137 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/udp137/udp_137_smb_nmap.txt" -oX "/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/udp137/xml/udp_137_smb_nmap.xml" 10.10.10.111

smbmap -H 10.10.10.111 -P 137 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 137 2>&1

smbmap -H 10.10.10.111 -P 137 -R 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 137 -R 2>&1

smbmap -H 10.10.10.111 -P 137 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.10.111 -P 137 -x "ipconfig /all" 2>&1


```