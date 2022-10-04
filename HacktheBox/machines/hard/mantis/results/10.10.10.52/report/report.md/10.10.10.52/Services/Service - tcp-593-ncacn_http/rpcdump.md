```bash
impacket-rpcdump -port 593 10.10.10.52
```

[/home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp593/tcp_593_rpc_rpcdump.txt](file:///home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/hard/mantis/results/10.10.10.52/scans/tcp593/tcp_593_rpc_rpcdump.txt):

```
Impacket v0.10.0 - Copyright 2022 SecureAuth Corporation

[*] Retrieving endpoint list from 10.10.10.52
Protocol: [MS-RSP]: Remote Shutdown Protocol
Provider: wininit.exe
UUID    : D95AFE70-A6D5-4259-822E-2C84DA1DDB0D v1.0
Bindings:
          ncacn_ip_tcp:10.10.10.52[49152]
          ncalrpc:[WindowsShutdown]
          ncacn_np:\\MANTIS[\PIPE\InitShutdown]
          ncalrpc:[WMsgKRpc08FF30]

Protocol: N/A
Provider: winlogon.exe
UUID    : 76F226C3-EC14-4325-8A99-6A46348418AF v1.0
Bindings:
          ncalrpc:[WindowsShutdown]
          ncacn_np:\\MANTIS[\PIPE\InitShutdown]
          ncalrpc:[WMsgKRpc08FF30]
          ncalrpc:[WMsgKRpc094A71]

Protocol: N/A
Provider: sysntfy.dll
UUID    : C9AC6DB5-82B7-4E55-AE8A-E464ED7B4277 v1.0 Impl friendly name
Bindings:
          ncalrpc:[LRPC-fb63918a43ba8791a0]
          ncalrpc:[senssvc]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]
          ncalrpc:[IUserProfile2]

Protocol: N/A
Provider: dhcpcsvc.dll
UUID    : 3C4728C5-F0AB-448B-BDA1-6CE01EB0A6D5 v1.0 DHCP Client LRPC Endpoint
Bindings:
          ncalrpc:[dhcpcsvc]
          ncalrpc:[dhcpcsvc6]
          ncacn_ip_tcp:10.10.10.52[49153]
          ncacn_np:\\MANTIS[\pipe\eventlog]
          ncalrpc:[eventlog]

Protocol: N/A
Provider: dhcpcsvc6.dll
UUID    : 3C4728C5-F0AB-448B-BDA1-6CE01EB0A6D6 v1.0 DHCPv6 Client LRPC Endpoint
Bindings:
          ncalrpc:[dhcpcsvc6]
          ncacn_ip_tcp:10.10.10.52[49153]
          ncacn_np:\\MANTIS[\pipe\eventlog]
          ncalrpc:[eventlog]

Protocol: N/A
Provider: nrpsrv.dll
UUID    : 30ADC50C-5CBC-46CE-9A0E-91914789E23C v1.0 NRP server endpoint
Bindings:
          ncacn_ip_tcp:10.10.10.52[49153]
          ncacn_np:\\MANTIS[\pipe\eventlog]
          ncalrpc:[eventlog]

Protocol: [MS-EVEN6]: EventLog Remoting Protocol
Provider: wevtsvc.dll
UUID    : F6BEAFF7-1E19-4FBB-9F8F-B89E2018337C v1.0 Event log TCPIP
Bindings:
          ncacn_ip_tcp:10.10.10.52[49153]
          ncacn_np:\\MANTIS[\pipe\eventlog]
          ncalrpc:[eventlog]

Protocol: N/A
Provider: srvsvc.dll
UUID    : 98716D03-89AC-44C7-BB8C-285824E51C4A v1.0 XactSrv service
Bindings:
          ncacn_ip_tcp:10.10.10.52[49154]
          ncacn_np:\\MANTIS[\PIPE\atsvc]
          ncalrpc:[senssvc]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]

Protocol: [MS-TSCH]: Task Scheduler Service Remoting Protocol
Provider: schedsvc.dll
UUID    : 86D35949-83C9-4044-B424-DB363231FD0C v1.0
Bindings:
          ncacn_ip_tcp:10.10.10.52[49154]
          ncacn_np:\\MANTIS[\PIPE\atsvc]
          ncalrpc:[senssvc]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]

Protocol: [MS-TSCH]: Task Scheduler Service Remoting Protocol
Provider: taskcomp.dll
UUID    : 378E52B0-C0A9-11CF-822D-00AA0051E40F v1.0
Bindings:
          ncacn_np:\\MANTIS[\PIPE\atsvc]
          ncalrpc:[senssvc]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]

Protocol: [MS-TSCH]: Task Scheduler Service Remoting Protocol
Provider: taskcomp.dll
UUID    : 1FF70682-0A51-30E8-076D-740BE8CEE98B v1.0
Bindings:
          ncacn_np:\\MANTIS[\PIPE\atsvc]
          ncalrpc:[senssvc]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]

Protocol: N/A
Provider: schedsvc.dll
UUID    : 0A74EF1C-41A4-4E06-83AE-DC74FB1CDD53 v1.0
Bindings:
          ncalrpc:[senssvc]
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]

Protocol: N/A
Provider: gpsvc.dll
UUID    : 2EB08E3E-639F-4FBA-97B1-14F878961076 v1.0
Bindings:
          ncalrpc:[OLE6813315BF93F4BE6A326006946AD]
          ncalrpc:[IUserProfile2]

Protocol: N/A
Provider: nsisvc.dll
UUID    : 7EA70BCF-48AF-4F6A-8968-6A440754D5FA v1.0 NSI server endpoint
Bindings:
          ncalrpc:[LRPC-5a35ff3a4070142ce4]
          ncalrpc:[OLEBAA4C073C762437DA84331DD3C9A]

Protocol: N/A
Provider: authui.dll
UUID    : 24019106-A203-4642-B88D-82DAE9158929 v1.0
Bindings:
          ncalrpc:[LRPC-985264a7552bd14fa2]

Protocol: N/A
Provider: MPSSVC.dll
UUID    : 2FB92682-6599-42DC-AE13-BD2CA89BD11C v1.0 Fw APIs
Bindings:
          ncalrpc:[LRPC-c0b3144c9e544f57c7]

Protocol: N/A
Provider: MPSSVC.dll
UUID    : 7F9D11BF-7FB9-436B-A812-B2D50C5D4C03 v1.0 Fw APIs
Bindings:
          ncalrpc:[LRPC-c0b3144c9e544f57c7]

Protocol: N/A
Provider: BFE.DLL
UUID    : DD490425-5325-4565-B774-7E27D6C09C24 v1.0 Base Firewall Engine API
Bindings:
          ncalrpc:[LRPC-c0b3144c9e544f57c7]

Protocol: [MS-SAMR]: Security Account Manager (SAM) Remote Protocol
Provider: samsrv.dll
UUID    : 12345778-1234-ABCD-EF00-0123456789AC v1.0
Bindings:
          ncacn_ip_tcp:10.10.10.52[49158]
          ncacn_http:10.10.10.52[49157]
          ncalrpc:[NTDS_LPC]
          ncalrpc:[OLEA86D5665F5AD418D92C63EB6B323]
          ncacn_ip_tcp:10.10.10.52[49155]
          ncalrpc:[samss lpc]
          ncalrpc:[dsrole]
          ncacn_np:\\MANTIS[\PIPE\protected_storage]
          ncalrpc:[protected_storage]
          ncalrpc:[lsasspirpc]
          ncalrpc:[lsapolicylookup]
          ncalrpc:[LSARPC_ENDPOINT]
          ncalrpc:[securityevent]
          ncalrpc:[audit]
          ncalrpc:[LRPC-445219c47fceb97cc9]
          ncacn_np:\\MANTIS[\pipe\lsass]

Protocol: [MS-LSAT]: Local Security Authority (Translation Methods) Remote
Provider: lsasrv.dll
UUID    : 12345778-1234-ABCD-EF00-0123456789AB v0.0
Bindings:
          ncacn_http:10.10.10.52[49157]
          ncalrpc:[NTDS_LPC]
          ncalrpc:[OLEA86D5665F5AD418D92C63EB6B323]
          ncacn_ip_tcp:10.10.10.52[49155]
          ncalrpc:[samss lpc]
          ncalrpc:[dsrole]
          ncacn_np:\\MANTIS[\PIPE\protected_storage]
          ncalrpc:[protected_storage]
          ncalrpc:[lsasspirpc]
          ncalrpc:[lsapolicylookup]
          ncalrpc:[LSARPC_ENDPOINT]
          ncalrpc:[securityevent]
          ncalrpc:[audit]
          ncalrpc:[LRPC-445219c47fceb97cc9]
          ncacn_np:\\MANTIS[\pipe\lsass]

Protocol: [MS-DRSR]: Directory Replication Service (DRS) Remote Protocol
Provider: ntdsai.dll
UUID    : E3514235-4B06-11D1-AB04-00C04FC2DCD2 v4.0 MS NT Directory DRS Interface
Bindings:
          ncacn_http:10.10.10.52[49157]
          ncalrpc:[NTDS_LPC]
          ncalrpc:[OLEA86D5665F5AD418D92C63EB6B323]
          ncacn_ip_tcp:10.10.10.52[49155]
          ncalrpc:[samss lpc]
          ncalrpc:[dsrole]
          ncacn_np:\\MANTIS[\PIPE\protected_storage]
          ncalrpc:[protected_storage]
          ncalrpc:[lsasspirpc]
          ncalrpc:[lsapolicylookup]
          ncalrpc:[LSARPC_ENDPOINT]
          ncalrpc:[securityevent]
          ncalrpc:[audit]
          ncalrpc:[LRPC-445219c47fceb97cc9]
          ncacn_np:\\MANTIS[\pipe\lsass]

[*] Received 105 endpoints.


```