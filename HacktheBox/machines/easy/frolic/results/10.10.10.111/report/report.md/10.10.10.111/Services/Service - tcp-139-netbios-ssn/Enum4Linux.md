```bash
enum4linux -a -M -l -d 10.10.10.111 2>&1
```

[/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp139/enum4linux.txt](file:///home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp139/enum4linux.txt):

```
Starting enum4linux v0.9.1 ( http://labs.portcullis.co.uk/application/enum4linux/ ) on Wed Nov 16 16:42:44 2022

[34m =========================================( [0m[32mTarget Information[0m[34m )=========================================

[0mTarget ........... 10.10.10.111
RID Range ........ 500-550,1000-1050
Username ......... ''
Password ......... ''
Known Usernames .. administrator, guest, krbtgt, domain admins, root, bin, none


[34m ============================( [0m[32mEnumerating Workgroup/Domain on 10.10.10.111[0m[34m )============================

[0m[33m
[+] [0m[32mGot domain/workgroup name: WORKGROUP

[0m
[34m ================================( [0m[32mNbtstat Information for 10.10.10.111[0m[34m )================================

[0mLooking up status of 10.10.10.111
	FROLIC          <00> -         B <ACTIVE>  Workstation Service
	FROLIC          <03> -         B <ACTIVE>  Messenger Service
	FROLIC          <20> -         B <ACTIVE>  File Server Service
	..__MSBROWSE__. <01> - <GROUP> B <ACTIVE>  Master Browser
	WORKGROUP       <00> - <GROUP> B <ACTIVE>  Domain/Workgroup Name
	WORKGROUP       <1d> -         B <ACTIVE>  Master Browser
	WORKGROUP       <1e> - <GROUP> B <ACTIVE>  Browser Service Elections

	MAC Address = 00-00-00-00-00-00

[34m ===================================( [0m[32mSession Check on 10.10.10.111[0m[34m )===================================

[0m[33m
[+] [0m[32mServer 10.10.10.111 allows sessions using username '', password ''

[0m
[34m ===========================( [0m[32mGetting information via LDAP for 10.10.10.111[0m[34m )===========================

[0m[33m
[+] [0m[32m10.10.10.111 appears to be a child DC

[0m
[34m ================================( [0m[32mGetting domain SID for 10.10.10.111[0m[34m )================================

[0mDomain Name: WORKGROUP
Domain Sid: (NULL SID)
[33m
[+] [0m[32mCan't determine if host is part of domain or part of a workgroup

[0m
[34m ===================================( [0m[32mOS information on 10.10.10.111[0m[34m )===================================

[0m[33m
[E] [0m[31mCan't get OS info with smbclient

[0m[33m
[+] [0m[32mGot OS info for 10.10.10.111 from srvinfo:
[0m	FROLIC         Wk Sv PrQ Unx NT SNT frolic server (Samba, Ubuntu)
	platform_id     :	500
	os version      :	6.1
	server type     :	0x809a03


[34m =======================================( [0m[32mUsers on 10.10.10.111[0m[34m )=======================================

[0mUse of uninitialized value $users in print at ./enum4linux.pl line 972.
Use of uninitialized value $users in pattern match (m//) at ./enum4linux.pl line 975.

Use of uninitialized value $users in print at ./enum4linux.pl line 986.
Use of uninitialized value $users in pattern match (m//) at ./enum4linux.pl line 988.

[34m ================================( [0m[32mMachine Enumeration on 10.10.10.111[0m[34m )================================

[0m[33m
[E] [0m[31mNot implemented in this version of enum4linux.

[0m
[34m =================================( [0m[32mShare Enumeration on 10.10.10.111[0m[34m )=================================

[0m
	Sharename       Type      Comment
	---------       ----      -------
	print$          Disk      Printer Drivers
	IPC$            IPC       IPC Service (frolic server (Samba, Ubuntu))
Reconnecting with SMB1 for workgroup listing.

	Server               Comment
	---------            -------

	Workgroup            Master
	---------            -------
	WORKGROUP            FROLIC
[33m
[+] [0m[32mAttempting to map shares on 10.10.10.111

[0m//10.10.10.111/print$	[35mMapping: [0mDENIED[35m Listing: [0mN/A[35m Writing: [0mN/A
[33m
[E] [0m[31mCan't understand response:

[0mNT_STATUS_OBJECT_NAME_NOT_FOUND listing \*
//10.10.10.111/IPC$	[35mMapping: [0mN/A[35m Listing: [0mN/A[35m Writing: [0mN/A

[34m ============================( [0m[32mPassword Policy Information for 10.10.10.111[0m[34m )============================

[0m

[+] Attaching to 10.10.10.111 using a NULL share

[+] Trying protocol 139/SMB...

[+] Found domain(s):

	[+] FROLIC
	[+] Builtin

[+] Password Info for Domain: FROLIC

	[+] Minimum password length: 5
	[+] Password history length: None
	[+] Maximum password age: Not Set
	[+] Password Complexity Flags: 000000

		[+] Domain Refuse Password Change: 0
		[+] Domain Password Store Cleartext: 0
		[+] Domain Password Lockout Admins: 0
		[+] Domain Password No Clear Change: 0
		[+] Domain Password No Anon Change: 0
		[+] Domain Password Complex: 0

	[+] Minimum password age: None
	[+] Reset Account Lockout Counter: 30 minutes
	[+] Locked Account Duration: 30 minutes
	[+] Account Lockout Threshold: None
	[+] Forced Log off Time: Not Set


[33m
[+] [0m[32mRetieved partial password policy with rpcclient:


[0mPassword Complexity: Disabled
Minimum Password Length: 5


[34m =======================================( [0m[32mGroups on 10.10.10.111[0m[34m )=======================================

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
[34m ==================( [0m[32mUsers on 10.10.10.111 via RID cycling (RIDS: 500-550,1000-1050)[0m[34m )==================

[0m[33m
[I] [0m[36mFound new SID:
[0mS-1-22-1
[33m
[I] [0m[36mFound new SID:
[0mS-1-5-32
[33m
[I] [0m[36mFound new SID:
[0mS-1-5-32
[33m
[I] [0m[36mFound new SID:
[0mS-1-5-32
[33m
[I] [0m[36mFound new SID:
[0mS-1-5-32
[33m
[+] [0m[32mEnumerating users using SID S-1-5-21-3106657666-1405957921-1930463546 and logon username '', password ''

[0mS-1-5-21-3106657666-1405957921-1930463546-501 FROLIC\nobody (Local User)
	User Name   :	nobody
	Full Name   :	nobody
	Home Drive  :
	Dir Drive   :	(null)
	Profile Path:
	Logon Script:
	Description :
	Workstations:
	Comment     :
	Remote Dial :
	Logon Time               :	Wed, 31 Dec 1969 19:00:00 EST
	Logoff Time              :	Wed, 13 Sep 30828 22:48:05 EDT
	Kickoff Time             :	Wed, 13 Sep 30828 22:48:05 EDT
	Password last set Time   :	Wed, 31 Dec 1969 19:00:00 EST
	Password can change Time :	Wed, 31 Dec 1969 19:00:00 EST
	Password must change Time:	Wed, 31 Dec 1969 19:00:00 EST
	unknown_2[0..31]...
	user_rid :	0x1f5
	group_rid:	0x201
	acb_info :	0x00000010
	fields_present:	0x00ffffff
	logon_divs:	168
	bad_password_count:	0x00000000
	logon_count:	0x00000000
	padding1[0..7]...
	logon_hrs[0..21]...
	Account Disabled         : False
	Password does not expire : False
	Account locked out       : False
	Password expired         : False
	Interdomain trust account: False
	Workstation trust account: False
	Server trust account     : False
	Trusted for delegation   : False

S-1-5-21-3106657666-1405957921-1930463546-513 FROLIC\None (Domain Group)
	Group Name:	None
	Description:	Ordinary Users
	Group Attribute:7
	Num Members:0

[33m
[+] [0m[32mEnumerating users using SID S-1-22-1 and logon username '', password ''

[0mS-1-22-1-1000 Unix User\sahay (Local User)
Use of uninitialized value $user_info in pattern match (m//) at ./enum4linux.pl line 1030.

S-1-22-1-1001 Unix User\ayush (Local User)
Use of uninitialized value $user_info in pattern match (m//) at ./enum4linux.pl line 1030.

[33m
[+] [0m[32mEnumerating users using SID S-1-5-32 and logon username '', password ''

[0mS-1-5-32-544 BUILTIN\Administrators (Local Group)
[33m
[E] [0m[31mNo info found


[0mS-1-5-32-545 BUILTIN\Users (Local Group)
[33m
[E] [0m[31mNo info found


[0mS-1-5-32-546 BUILTIN\Guests (Local Group)
[33m
[E] [0m[31mNo info found


[0mS-1-5-32-547 BUILTIN\Power Users (Local Group)
[33m
[E] [0m[31mNo info found


[0mS-1-5-32-548 BUILTIN\Account Operators (Local Group)
[33m
[E] [0m[31mNo info found


[0mS-1-5-32-549 BUILTIN\Server Operators (Local Group)
[33m
[E] [0m[31mNo info found


[0mS-1-5-32-550 BUILTIN\Print Operators (Local Group)
[33m
[E] [0m[31mNo info found


[0m
[34m ===============================( [0m[32mGetting printer info for 10.10.10.111[0m[34m )===============================

[0mNo printers returned.


enum4linux complete on Wed Nov 16 16:44:00 2022



```
