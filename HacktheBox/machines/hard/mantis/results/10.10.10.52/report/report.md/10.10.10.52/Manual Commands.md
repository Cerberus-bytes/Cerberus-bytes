```bash
[*] msrpc on tcp/135

	[-] RPC Client:

		rpcclient -p 135 -U "" 10.10.10.52

[*] netbios-ssn on tcp/139

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -sV -p 139 --script="smb-vuln-ms06-025" --script-args="unsafe=1" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp139/tcp_139_smb_ms06-025.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp139/xml/tcp_139_smb_ms06-025.xml" 10.10.10.52

		nmap -vv --reason -Pn -T4 -sV -p 139 --script="smb-vuln-ms07-029" --script-args="unsafe=1" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp139/tcp_139_smb_ms07-029.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp139/xml/tcp_139_smb_ms07-029.xml" 10.10.10.52

		nmap -vv --reason -Pn -T4 -sV -p 139 --script="smb-vuln-ms08-067" --script-args="unsafe=1" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp139/tcp_139_smb_ms08-067.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp139/xml/tcp_139_smb_ms08-067.xml" 10.10.10.52

[*] ldap on tcp/389

	[-] ldapsearch command (modify before running):

		ldapsearch -x -D "<username>" -w "<password>" -H ldap://10.10.10.52:389 -b "dc=example,dc=com" -s sub "(objectclass=*)" 2>&1 | tee > "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp389/tcp_389_ldap_all-entries.txt"

[*] msrpc on tcp/49152

	[-] RPC Client:

		rpcclient -p 49152 -U "" 10.10.10.52

[*] msrpc on tcp/49153

	[-] RPC Client:

		rpcclient -p 49153 -U "" 10.10.10.52

[*] msrpc on tcp/49154

	[-] RPC Client:

		rpcclient -p 49154 -U "" 10.10.10.52

[*] msrpc on tcp/49155

	[-] RPC Client:

		rpcclient -p 49155 -U "" 10.10.10.52

[*] msrpc on tcp/49158

	[-] RPC Client:

		rpcclient -p 49158 -U "" 10.10.10.52


```