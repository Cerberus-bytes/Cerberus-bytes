```bash
whatweb --color=never --no-errors -a 3 -v http://10.10.10.111:9999 2>&1
```

[/home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp9999/tcp_9999_http_whatweb.txt](file:///home/Default/Documents/Repos/cerberus-bytes/Cerberus-bytes/HacktheBox/machines/easy/frolic/results/10.10.10.111/scans/tcp9999/tcp_9999_http_whatweb.txt):

```
WhatWeb report for http://10.10.10.111:9999
Status    : 200 OK
Title     : Welcome to nginx!
IP        : 10.10.10.111
Country   : RESERVED, ZZ

Summary   : HTML5, HTTPServer[Ubuntu Linux][nginx/1.10.3 (Ubuntu)], nginx[1.10.3]

Detected Plugins:
[ HTML5 ]
	HTML version 5, detected by the doctype declaration


[ HTTPServer ]
	HTTP server header string. This plugin also attempts to
	identify the operating system from the server header.

	OS           : Ubuntu Linux
	String       : nginx/1.10.3 (Ubuntu) (from server string)

[ nginx ]
	Nginx (Engine-X) is a free, open-source, high-performance
	HTTP server and reverse proxy, as well as an IMAP/POP3
	proxy server.

	Version      : 1.10.3
	Website     : http://nginx.net/

HTTP Headers:
	HTTP/1.1 200 OK
	Server: nginx/1.10.3 (Ubuntu)
	Date: Wed, 16 Nov 2022 21:42:50 GMT
	Content-Type: text/html
	Last-Modified: Sun, 23 Sep 2018 12:03:28 GMT
	Transfer-Encoding: chunked
	Connection: close
	ETag: W/"5ba78110-27d"
	Content-Encoding: gzip



```
