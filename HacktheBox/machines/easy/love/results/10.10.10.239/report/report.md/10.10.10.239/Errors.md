```
[*] Service scan SMBClient (tcp/445/microsoft-ds/smbclient) ran a command which returned a non-zero exit code (1).
[-] Command: smbclient -L //10.10.10.239 -N -I 10.10.10.239 2>&1
[-] Error Output:


[*] Service scan wkhtmltoimage (tcp/443/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png https://10.10.10.239:443/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/love/results/10.10.10.239/scans/tcp443/tcp_443_https_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Warning: SSL error ignored
Error: Failed to load https://10.10.10.239/, with network status code 201 and http status code 403 - Error transferring https://10.10.10.239/ - server replied: Forbidden
[==============================>                             ] 50%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentAccessDenied


[*] Service scan wkhtmltoimage (tcp/5000/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png http://10.10.10.239:5000/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/love/results/10.10.10.239/scans/tcp5000/tcp_5000_http_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Error: Failed to load http://10.10.10.239:5000/, with network status code 201 and http status code 403 - Error transferring http://10.10.10.239:5000/ - server replied: Forbidden
[==============================>                             ] 50%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentAccessDenied


[*] Service scan Enum4Linux (tcp/445/microsoft-ds/enum4linux) ran a command which returned a non-zero exit code (1).
[-] Command: enum4linux -a -M -l -d 10.10.10.239 2>&1
[-] Error Output:


[*] Service scan wkhtmltoimage (tcp/5985/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png http://10.10.10.239:5985/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/love/results/10.10.10.239/scans/tcp5985/tcp_5985_http_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Error: Failed to load http://10.10.10.239:5985/, with network status code 203 and http status code 404 - Error transferring http://10.10.10.239:5985/ - server replied: Not Found
[==============================>                             ] 50%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentNotFoundError


[*] Service scan wkhtmltoimage (tcp/47001/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png http://10.10.10.239:47001/ /home/Default/Documents/Repos/Default_/Platforms/HacktheBox/machines/easy/love/results/10.10.10.239/scans/tcp47001/tcp_47001_http_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Error: Failed to load http://10.10.10.239:47001/, with network status code 203 and http status code 404 - Error transferring http://10.10.10.239:47001/ - server replied: Not Found
[==============================>                             ] 50%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentNotFoundError



```