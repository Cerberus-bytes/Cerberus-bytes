```bash
nmap -vv --reason -Pn -T4 -sV -p 389 --script="banner,(ldap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/tcp_389_ldap_nmap.txt" -oX "/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/xml/tcp_389_ldap_nmap.xml" 10.10.10.172
```

[/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/tcp_389_ldap_nmap.txt](file:///home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/tcp_389_ldap_nmap.txt):

```
# Nmap 7.92 scan initiated Tue Sep 20 18:59:04 2022 as: nmap -vv --reason -Pn -T4 -sV -p 389 "--script=banner,(ldap* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/tcp_389_ldap_nmap.txt -oX /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/medium/monteverde/results/10.10.10.172/scans/tcp389/xml/tcp_389_ldap_nmap.xml 10.10.10.172
Nmap scan report for 10.10.10.172
Host is up, received user-set (0.029s latency).
Scanned at 2022-09-20 18:59:05 EDT for 16s

PORT    STATE SERVICE REASON          VERSION
389/tcp open  ldap    syn-ack ttl 127 Microsoft Windows Active Directory LDAP (Domain: MEGABANK.LOCAL, Site: Default-First-Site-Name)
| ldap-search: 
|   Context: DC=MEGABANK,DC=LOCAL
|     dn: DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: domain
|         objectClass: domainDNS
|         distinguishedName: DC=MEGABANK,DC=LOCAL
|         instanceType: 5
|         whenCreated: 2020/01/02 22:05:15 UTC
|         whenChanged: 2022/09/20 22:49:53 UTC
|         subRefs: DC=ForestDnsZones,DC=MEGABANK,DC=LOCAL
|         subRefs: DC=DomainDnsZones,DC=MEGABANK,DC=LOCAL
|         subRefs: CN=Configuration,DC=MEGABANK,DC=LOCAL
|         uSNCreated: 4099
|         dSASignature: \x01\x00\x00\x00(\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x0F{\xA0:\xC3/1O\x86J\xDD\xEC\xA2\xD3\\xC5
|         uSNChanged: 69657
|         name: MEGABANK
|         objectGUID: 41195d74-6f66-9846-ba78-67509841f4d0
|         replUpToDateVector: \x02\x00\x00\x00\x00\x00\x00\x00	\x00\x00\x00\x00\x00\x00\x00\x0F{\xA0:\xC3/1O\x86J\xDD\xEC\xA2\xD3\\xC5\x05p\x00\x00\x00\x00\x00\x00x\x0C\x1F\x14\x03\x00\x00\x003\xA0\x84H\xAB\xEA\x83D\xB2\xF1	\xF6\xEF0\x8Ex
|         \xC0\x00\x00\x00\x00\x00\x00\xB1\xF3\x1F\x14\x03\x00\x00\x00LE4U2C!C\xA9\x0B\xE9\xAE\xCFU\x86\x1C\x0C\xE0\x00\x00\x00\x00\x00\x00\x15\xCD#\x14\x03\x00\x00\x00eS2XR\xA9\A\xADpF\xD4S\xEF\xEAX	\xB0\x00\x00\x00\x00\x00\x00\x07\xE7\x1F\x14\x03\x00\x00\x00^\xFD\xEBv\x1F\xD5\x9AL\x8Eq)\xA6\x87[\x8D\xCB\x0E\x00\x01\x00\x00\x00\x00\x00M\xCE\xB2\x16\x03\x00\x00\x00\x87?\x16\x90n=\xFFG\xAC\x94\x0F\xEFKz
|         \x8E\x07\x90\x00\x00\x00\x00\x00\x00\xE4\x16\x1F\x14\x03\x00\x00\x00\x0F\x9F\xF7\xE4\xCE\xE3ZD\xAB	:\x88\xCF\xC9\x04\xC9\x06\x80\x00\x00\x00\x00\x00\x009\x13\x1F\x14\x03\x00\x00\x00\xA7_I\xF0\x03\xAAbK\xBC7\x87\x176#r\xA7\x0B\xD0\x00\x00\x00\x00\x00\x00\xBA\x99#\x14\x03\x00\x00\x00IB\xC3\xF8h\x07AO\x8E\x01c\xEC\xEC\x848!\x0F\x10\x01\x00\x00\x00\x00\x00\x90\xD4:\x19\x03\x00\x00\x00
|         creationTime: 133081877939584483
|         forceLogoff: -9223372036854775808
|         lockoutDuration: -18000000000
|         lockOutObservationWindow: -18000000000
|         lockoutThreshold: 0
|         maxPwdAge: -36288000000000
|         minPwdAge: -864000000000
|         minPwdLength: 7
|         modifiedCountAtLastProm: 0
|         nextRid: 1000
|         pwdProperties: 0
|         pwdHistoryLength: 24
|         objectSid: 1-5-21-391775091-850290835-3566037492
|         serverState: 1
|         uASCompat: 1
|         modifiedCount: 1
|         auditingPolicy: \x00\x01
|         nTMixedDomain: 0
|         rIDManagerReference: CN=RID Manager$,CN=System,DC=MEGABANK,DC=LOCAL
|         fSMORoleOwner: CN=NTDS Settings,CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         systemFlags: -1946157056
|         wellKnownObjects: B:32:6227F0AF1FC2410D8E3BB10615BB5B0F:CN=NTDS Quotas,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:F4BE92A4C777485E878E9421D53087DB:CN=Microsoft,CN=Program Data,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:09460C08AE1E4A4EA0F64AEE7DAA1E5A:CN=Program Data,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:22B70C67D56E4EFB91E9300FCA3DC1AA:CN=ForeignSecurityPrincipals,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:18E2EA80684F11D2B9AA00C04F79F805:CN=Deleted Objects,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:2FBAC1870ADE11D297C400C04FD8D5CD:CN=Infrastructure,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:AB8153B7768811D1ADED00C04FD8D5CD:CN=LostAndFound,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:AB1D30F3768811D1ADED00C04FD8D5CD:CN=System,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:A361B2FFFFD211D1AA4B00C04FD7D83A:OU=Domain Controllers,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:AA312825768811D1ADED00C04FD8D5CD:CN=Computers,DC=MEGABANK,DC=LOCAL
|         wellKnownObjects: B:32:A9D1CA15768811D1ADED00C04FD8D5CD:CN=Users,DC=MEGABANK,DC=LOCAL
|         objectCategory: CN=Domain-DNS,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         gPLink: [LDAP://CN={31B2F340-016D-11D2-945F-00C04FB984F9},CN=Policies,CN=System,DC=MEGABANK,DC=LOCAL;0]
|         dSCorePropagationData: 1601/01/01 00:00:00 UTC
|         otherWellKnownObjects: B:32:683A24E2E8164BD3AF86AC3C2CF3F981:CN=Keys,DC=MEGABANK,DC=LOCAL
|         otherWellKnownObjects: B:32:1EB93889E40C45DF9F0C64D23BBB6237:CN=Managed Service Accounts,DC=MEGABANK,DC=LOCAL
|         masteredBy: CN=NTDS Settings,CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         ms-DS-MachineAccountQuota: 10
|         msDS-Behavior-Version: 7
|         msDS-PerUserTrustQuota: 1
|         msDS-AllUsersTrustQuota: 1000
|         msDS-PerUserTrustTombstonesQuota: 10
|         msDs-masteredBy: CN=NTDS Settings,CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         msDS-IsDomainFor: CN=NTDS Settings,CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         msDS-NcType: 0
|         msDS-ExpirePasswordsOnSmartCardOnlyAccounts: TRUE
|         dc: MEGABANK
|     dn: CN=Users,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: Users
|         description: Default container for upgraded user accounts
|         distinguishedName: CN=Users,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5660
|         uSNChanged: 5660
|         showInAdvancedViewOnly: FALSE
|         name: Users
|         objectGUID: ed111f21-9bda-7848-99e3-7822fc4a7877
|         systemFlags: -1946157056
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=Computers,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: Computers
|         description: Default container for upgraded computer accounts
|         distinguishedName: CN=Computers,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5661
|         uSNChanged: 5661
|         showInAdvancedViewOnly: FALSE
|         name: Computers
|         objectGUID: e1361e19-4827-7341-b494-5c92773423b
|         systemFlags: -1946157056
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: OU=Domain Controllers,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: organizationalUnit
|         ou: Domain Controllers
|         description: Default container for domain controllers
|         distinguishedName: OU=Domain Controllers,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5804
|         uSNChanged: 5804
|         showInAdvancedViewOnly: FALSE
|         name: Domain Controllers
|         objectGUID: 69cd410-dd9d-9a4f-a116-b9c4659bf311
|         systemFlags: -1946157056
|         objectCategory: CN=Organizational-Unit,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         gPLink: [LDAP://CN={6AC1786C-016F-11D2-945F-00C04fB984F9},CN=Policies,CN=System,DC=MEGABANK,DC=LOCAL;0]
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: System
|         description: Builtin system settings
|         distinguishedName: CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5662
|         uSNChanged: 5662
|         showInAdvancedViewOnly: TRUE
|         name: System
|         objectGUID: d4bef35-c7e1-2244-820-cbbdb1e75a6c
|         systemFlags: -1946157056
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=LostAndFound,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: lostAndFound
|         cn: LostAndFound
|         description: Default container for orphaned objects
|         distinguishedName: CN=LostAndFound,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5658
|         uSNChanged: 5658
|         showInAdvancedViewOnly: TRUE
|         name: LostAndFound
|         objectGUID: e44f8b66-9e2-b743-98fb-7167f0cc30f6
|         systemFlags: -1946157056
|         objectCategory: CN=Lost-And-Found,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=Infrastructure,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: infrastructureUpdate
|         cn: Infrastructure
|         distinguishedName: CN=Infrastructure,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5805
|         uSNChanged: 5805
|         showInAdvancedViewOnly: TRUE
|         name: Infrastructure
|         objectGUID: 3951ff4c-bfd5-140-ba7-293eba1df2ae
|         fSMORoleOwner: CN=NTDS Settings,CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         systemFlags: -1946157056
|         objectCategory: CN=Infrastructure-Update,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=ForeignSecurityPrincipals,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: ForeignSecurityPrincipals
|         description: Default container for security identifiers (SIDs) associated with objects from external, trusted domains
|         distinguishedName: CN=ForeignSecurityPrincipals,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5806
|         uSNChanged: 5806
|         showInAdvancedViewOnly: FALSE
|         name: ForeignSecurityPrincipals
|         objectGUID: 80b128a-446-bb4c-8eb1-b05ddaba6cc
|         systemFlags: -1946157056
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=Program Data,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: Program Data
|         description: Default location for storage of application data.
|         distinguishedName: CN=Program Data,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5807
|         uSNChanged: 5807
|         showInAdvancedViewOnly: TRUE
|         name: Program Data
|         objectGUID: 22a15d25-f9d-f642-a776-34eb757e150
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=Microsoft,CN=Program Data,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: Microsoft
|         description: Default location for storage of Microsoft application data.
|         distinguishedName: CN=Microsoft,CN=Program Data,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5808
|         uSNChanged: 5808
|         showInAdvancedViewOnly: TRUE
|         name: Microsoft
|         objectGUID: d3a156a5-c8dc-6c4a-b34e-3f45c6122f5b
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
|     dn: CN=NTDS Quotas,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: msDS-QuotaContainer
|         cn: NTDS Quotas
|         description: Quota specifications container
|         distinguishedName: CN=NTDS Quotas,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5809
|         uSNChanged: 5809
|         showInAdvancedViewOnly: TRUE
|         name: NTDS Quotas
|         objectGUID: e46dbe8c-39b0-f542-b78d-b62a9e6e79a
|         systemFlags: -2147483648
|         objectCategory: CN=ms-DS-Quota-Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|         msDS-TombstoneQuotaFactor: 100
|     dn: CN=Managed Service Accounts,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: Managed Service Accounts
|         description: Default container for managed service accounts
|         distinguishedName: CN=Managed Service Accounts,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:22 UTC
|         whenChanged: 2020/01/02 22:05:22 UTC
|         uSNCreated: 5810
|         uSNChanged: 5810
|         showInAdvancedViewOnly: FALSE
|         name: Managed Service Accounts
|         objectGUID: a4396113-6224-2349-8a7d-43e0f37541a6
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:44:45 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 18:12:17 UTC
|     dn: CN=Keys,DC=MEGABANK,DC=LOCAL
|     dn: CN=WinsockServices,CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         cn: WinsockServices
|         distinguishedName: CN=WinsockServices,CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5663
|         uSNChanged: 5663
|         showInAdvancedViewOnly: TRUE
|         name: WinsockServices
|         objectGUID: d0a3d233-2c86-774d-8868-10e1ea567212
|         objectCategory: CN=Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
|     dn: CN=RpcServices,CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: container
|         objectClass: rpcContainer
|         cn: RpcServices
|         distinguishedName: CN=RpcServices,CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5664
|         uSNChanged: 5664
|         showInAdvancedViewOnly: TRUE
|         name: RpcServices
|         objectGUID: 5fd7aad9-2b75-da4b-87d0-277c33dca49
|         systemFlags: -1946157056
|         objectCategory: CN=Rpc-Container,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
|     dn: CN=FileLinks,CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: fileLinkTracking
|         cn: FileLinks
|         distinguishedName: CN=FileLinks,CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5665
|         uSNChanged: 5665
|         showInAdvancedViewOnly: TRUE
|         name: FileLinks
|         objectGUID: 6c75110-cdd4-ae4c-8989-f0b359f3122f
|         systemFlags: -1946157056
|         objectCategory: CN=File-Link-Tracking,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
|     dn: CN=VolumeTable,CN=FileLinks,CN=System,DC=MEGABANK,DC=LOCAL
|     dn: CN=ObjectMoveTable,CN=FileLinks,CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: fileLinkTracking
|         objectClass: linkTrackObjectMoveTable
|         cn: ObjectMoveTable
|         distinguishedName: CN=ObjectMoveTable,CN=FileLinks,CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5667
|         uSNChanged: 5667
|         showInAdvancedViewOnly: TRUE
|         name: ObjectMoveTable
|         objectGUID: fd7ffc6-23f4-8a45-a93a-732a658e15b
|         systemFlags: -1946157056
|         objectCategory: CN=Link-Track-Object-Move-Table,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
|     dn: CN=Default Domain Policy,CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: leaf
|         objectClass: domainPolicy
|         cn: Default Domain Policy
|         distinguishedName: CN=Default Domain Policy,CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5668
|         uSNChanged: 5668
|         showInAdvancedViewOnly: TRUE
|         name: Default Domain Policy
|         objectGUID: 4ebec328-9770-d149-8580-b87802e8ee
|         objectCategory: CN=Domain-Policy,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
|     dn: CN=AppCategories,CN=Default Domain Policy,CN=System,DC=MEGABANK,DC=LOCAL
|         objectClass: top
|         objectClass: classStore
|         cn: AppCategories
|         distinguishedName: CN=AppCategories,CN=Default Domain Policy,CN=System,DC=MEGABANK,DC=LOCAL
|         instanceType: 4
|         whenCreated: 2020/01/02 22:05:21 UTC
|         whenChanged: 2020/01/02 22:05:21 UTC
|         uSNCreated: 5669
|         uSNChanged: 5669
|         showInAdvancedViewOnly: TRUE
|         name: AppCategories
|         objectGUID: cee13c8a-7b0-2e4d-9fa-a8d1f2a763c9
|         objectCategory: CN=Class-Store,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|         isCriticalSystemObject: TRUE
|         dSCorePropagationData: 2020/01/03 12:35:51 UTC
|         dSCorePropagationData: 2020/01/02 22:06:03 UTC
|         dSCorePropagationData: 1601/01/01 00:04:17 UTC
| 
| 
|_Result limited to 20 objects (see ldap.maxobjects)
| ldap-rootdse: 
| LDAP Results
|   <ROOT>
|       domainFunctionality: 7
|       forestFunctionality: 7
|       domainControllerFunctionality: 7
|       rootDomainNamingContext: DC=MEGABANK,DC=LOCAL
|       ldapServiceName: MEGABANK.LOCAL:monteverde$@MEGABANK.LOCAL
|       isGlobalCatalogReady: TRUE
|       supportedSASLMechanisms: GSSAPI
|       supportedSASLMechanisms: GSS-SPNEGO
|       supportedSASLMechanisms: EXTERNAL
|       supportedSASLMechanisms: DIGEST-MD5
|       supportedLDAPVersion: 3
|       supportedLDAPVersion: 2
|       supportedLDAPPolicies: MaxPoolThreads
|       supportedLDAPPolicies: MaxPercentDirSyncRequests
|       supportedLDAPPolicies: MaxDatagramRecv
|       supportedLDAPPolicies: MaxReceiveBuffer
|       supportedLDAPPolicies: InitRecvTimeout
|       supportedLDAPPolicies: MaxConnections
|       supportedLDAPPolicies: MaxConnIdleTime
|       supportedLDAPPolicies: MaxPageSize
|       supportedLDAPPolicies: MaxBatchReturnMessages
|       supportedLDAPPolicies: MaxQueryDuration
|       supportedLDAPPolicies: MaxDirSyncDuration
|       supportedLDAPPolicies: MaxTempTableSize
|       supportedLDAPPolicies: MaxResultSetSize
|       supportedLDAPPolicies: MinResultSets
|       supportedLDAPPolicies: MaxResultSetsPerConn
|       supportedLDAPPolicies: MaxNotificationPerConn
|       supportedLDAPPolicies: MaxValRange
|       supportedLDAPPolicies: MaxValRangeTransitive
|       supportedLDAPPolicies: ThreadMemoryLimit
|       supportedLDAPPolicies: SystemMemoryLimitPercent
|       supportedControl: 1.2.840.113556.1.4.319
|       supportedControl: 1.2.840.113556.1.4.801
|       supportedControl: 1.2.840.113556.1.4.473
|       supportedControl: 1.2.840.113556.1.4.528
|       supportedControl: 1.2.840.113556.1.4.417
|       supportedControl: 1.2.840.113556.1.4.619
|       supportedControl: 1.2.840.113556.1.4.841
|       supportedControl: 1.2.840.113556.1.4.529
|       supportedControl: 1.2.840.113556.1.4.805
|       supportedControl: 1.2.840.113556.1.4.521
|       supportedControl: 1.2.840.113556.1.4.970
|       supportedControl: 1.2.840.113556.1.4.1338
|       supportedControl: 1.2.840.113556.1.4.474
|       supportedControl: 1.2.840.113556.1.4.1339
|       supportedControl: 1.2.840.113556.1.4.1340
|       supportedControl: 1.2.840.113556.1.4.1413
|       supportedControl: 2.16.840.1.113730.3.4.9
|       supportedControl: 2.16.840.1.113730.3.4.10
|       supportedControl: 1.2.840.113556.1.4.1504
|       supportedControl: 1.2.840.113556.1.4.1852
|       supportedControl: 1.2.840.113556.1.4.802
|       supportedControl: 1.2.840.113556.1.4.1907
|       supportedControl: 1.2.840.113556.1.4.1948
|       supportedControl: 1.2.840.113556.1.4.1974
|       supportedControl: 1.2.840.113556.1.4.1341
|       supportedControl: 1.2.840.113556.1.4.2026
|       supportedControl: 1.2.840.113556.1.4.2064
|       supportedControl: 1.2.840.113556.1.4.2065
|       supportedControl: 1.2.840.113556.1.4.2066
|       supportedControl: 1.2.840.113556.1.4.2090
|       supportedControl: 1.2.840.113556.1.4.2205
|       supportedControl: 1.2.840.113556.1.4.2204
|       supportedControl: 1.2.840.113556.1.4.2206
|       supportedControl: 1.2.840.113556.1.4.2211
|       supportedControl: 1.2.840.113556.1.4.2239
|       supportedControl: 1.2.840.113556.1.4.2255
|       supportedControl: 1.2.840.113556.1.4.2256
|       supportedControl: 1.2.840.113556.1.4.2309
|       supportedControl: 1.2.840.113556.1.4.2330
|       supportedControl: 1.2.840.113556.1.4.2354
|       supportedCapabilities: 1.2.840.113556.1.4.800
|       supportedCapabilities: 1.2.840.113556.1.4.1670
|       supportedCapabilities: 1.2.840.113556.1.4.1791
|       supportedCapabilities: 1.2.840.113556.1.4.1935
|       supportedCapabilities: 1.2.840.113556.1.4.2080
|       supportedCapabilities: 1.2.840.113556.1.4.2237
|       subschemaSubentry: CN=Aggregate,CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|       serverName: CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|       schemaNamingContext: CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|       namingContexts: DC=MEGABANK,DC=LOCAL
|       namingContexts: CN=Configuration,DC=MEGABANK,DC=LOCAL
|       namingContexts: CN=Schema,CN=Configuration,DC=MEGABANK,DC=LOCAL
|       namingContexts: DC=DomainDnsZones,DC=MEGABANK,DC=LOCAL
|       namingContexts: DC=ForestDnsZones,DC=MEGABANK,DC=LOCAL
|       isSynchronized: TRUE
|       highestCommittedUSN: 69692
|       dsServiceName: CN=NTDS Settings,CN=MONTEVERDE,CN=Servers,CN=Default-First-Site-Name,CN=Sites,CN=Configuration,DC=MEGABANK,DC=LOCAL
|       dnsHostName: MONTEVERDE.MEGABANK.LOCAL
|       defaultNamingContext: DC=MEGABANK,DC=LOCAL
|       currentTime: 20220920225911.0Z
|_      configurationNamingContext: CN=Configuration,DC=MEGABANK,DC=LOCAL
Service Info: Host: MONTEVERDE; OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Tue Sep 20 18:59:21 2022 -- 1 IP address (1 host up) scanned in 17.25 seconds

```
