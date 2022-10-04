```bash
enum4linux -a -M -l -d 10.10.10.100 2>&1
```

[/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/active/results/10.10.10.100/scans/tcp139/enum4linux.txt](file:///home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/active/results/10.10.10.100/scans/tcp139/enum4linux.txt):

```
Starting enum4linux v0.9.1 ( http://labs.portcullis.co.uk/application/enum4linux/ ) on Mon Sep 19 18:45:09 2022

[34m =========================================( [0m[32mTarget Information[0m[34m )=========================================

[0mTarget ........... 10.10.10.100
RID Range ........ 500-550,1000-1050
Username ......... ''
Password ......... ''
Known Usernames .. administrator, guest, krbtgt, domain admins, root, bin, none


[34m ============================( [0m[32mEnumerating Workgroup/Domain on 10.10.10.100[0m[34m )============================

[0m[33m
[E] [0m[31mCan't find workgroup/domain

[0m

[34m ================================( [0m[32mNbtstat Information for 10.10.10.100[0m[34m )================================

[0mLooking up status of 10.10.10.100
No reply from 10.10.10.100

[34m ===================================( [0m[32mSession Check on 10.10.10.100[0m[34m )===================================

[0m[33m
[+] [0m[32mServer 10.10.10.100 allows sessions using username '', password ''

[0m
[34m ===========================( [0m[32mGetting information via LDAP for 10.10.10.100[0m[34m )===========================

[0m[33m
[+] [0m[32m10.10.10.100 appears to be a child DC

[0m
[34m ================================( [0m[32mGetting domain SID for 10.10.10.100[0m[34m )================================

[0mdo_cmd: Could not initialise lsarpc. Error was NT_STATUS_ACCESS_DENIED
[33m
[+] [0m[32mCan't determine if host is part of domain or part of a workgroup

[0m
[34m ===================================( [0m[32mOS information on 10.10.10.100[0m[34m )===================================

[0m[33m
[E] [0m[31mCan't get OS info with smbclient

[0m[33m
[+] [0m[32mGot OS info for 10.10.10.100 from srvinfo:
[0m	10.10.10.100   Wk Sv PDC Tim NT     Domain Controller
	platform_id     :	500
	os version      :	6.1
	server type     :	0x80102b


[34m =======================================( [0m[32mUsers on 10.10.10.100[0m[34m )=======================================

[0m[33m
[E] [0m[31mCouldn't find users using querydispinfo: NT_STATUS_ACCESS_DENIED

[0m
[33m
[E] [0m[31mCouldn't find users using enumdomusers: NT_STATUS_ACCESS_DENIED

[0m
[34m ================================( [0m[32mMachine Enumeration on 10.10.10.100[0m[34m )================================

[0m[33m
[E] [0m[31mNot implemented in this version of enum4linux.

[0m
[34m =================================( [0m[32mShare Enumeration on 10.10.10.100[0m[34m )=================================

[0mdo_connect: Connection to 10.10.10.100 failed (Error NT_STATUS_RESOURCE_NAME_NOT_FOUND)

	Sharename       Type      Comment
	---------       ----      -------
	ADMIN$          Disk      Remote Admin
	C$              Disk      Default share
	IPC$            IPC       Remote IPC
	NETLOGON        Disk      Logon server share
	Replication     Disk
	SYSVOL          Disk      Logon server share
	Users           Disk
Reconnecting with SMB1 for workgroup listing.
Unable to connect with SMB1 -- no workgroup available
[33m
[+] [0m[32mAttempting to map shares on 10.10.10.100

[0m//10.10.10.100/ADMIN$	[35mMapping: [0mDENIED[35m Listing: [0mN/A[35m Writing: [0mN/A
//10.10.10.100/C$	[35mMapping: [0mDENIED[35m Listing: [0mN/A[35m Writing: [0mN/A
//10.10.10.100/IPC$	[35mMapping: [0mOK[35m Listing: [0mDENIED[35m Writing: [0mN/A
//10.10.10.100/NETLOGON	[35mMapping: [0mDENIED[35m Listing: [0mN/A[35m Writing: [0mN/A
//10.10.10.100/Replication	[35mMapping: [0mOK[35m Listing: [0mOK[35m Writing: [0mN/A
//10.10.10.100/SYSVOL	[35mMapping: [0mDENIED[35m Listing: [0mN/A[35m Writing: [0mN/A
//10.10.10.100/Users	[35mMapping: [0mDENIED[35m Listing: [0mN/A[35m Writing: [0mN/A

[34m ============================( [0m[32mPassword Policy Information for 10.10.10.100[0m[34m )============================

[0m[33m
[E] [0m[31mUnexpected error from polenum:

[0m

[+] Attaching to 10.10.10.100 using a NULL share

[+] Trying protocol 139/SMB...

	[!] Protocol failed: Cannot request session (Called Name:10.10.10.100)

[+] Trying protocol 445/SMB...

	[!] Protocol failed: SMB SessionError: STATUS_ACCESS_DENIED({Access Denied} A process has requested access to an object but has not been granted those access rights.)


[33m
[E] [0m[31mFailed to get password policy with rpcclient

[0m

[34m =======================================( [0m[32mGroups on 10.10.10.100[0m[34m )=======================================

[0m[33m
[+] [0m[32mGetting builtin groups:

[0m[33m
[+] [0m[32m Getting builtin group memberships:

[0m[33m
[+] [0m[32m Getting local groups:

[0m[33m
[+] [0m[32m Getting local group memberships:

[0m[33m
[+] [0m[32m Getting domain groups:

[0m[33m
[+] [0m[32m Getting domain group memberships:

[0m
[34m ==================( [0m[32mUsers on 10.10.10.100 via RID cycling (RIDS: 500-550,1000-1050)[0m[34m )==================

[0m[33m
[E] [0m[31mCouldn't get SID: NT_STATUS_ACCESS_DENIED.  RID cycling not possible.

[0m
[34m ===============================( [0m[32mGetting printer info for 10.10.10.100[0m[34m )===============================

[0mdo_cmd: Could not initialise spoolss. Error was NT_STATUS_ACCESS_DENIED


enum4linux complete on Mon Sep 19 18:45:33 2022



```