#Hilfreiche Befehle

- **ipconfig** zeigt einem die aktuelle IP Konfiguration an
```cmd
ipconfig 
```
- **ipconfig /all** zeigt einem erweiterte Informationen zur IP Konfiguration an wie z.B. Lease Dauer und DHCP Server
```cmd
ipconfig /all
```

- **nslookup** ermöglicht manuelle DNS Abfragen in der "alten" Kommandozeile. 
```cmd
nslookup ppedv.de
```
Alternativ in der PowerShell:
```powershell
Resolve-DnsName -Name ppedv.de
```
Weitere Parameter und Verwendung [Link zu MicrosoftDocs](https://docs.microsoft.com/en-us/powershell/module/dnsclient/resolve-dnsname?view=windowsserver2022-ps)

- **ipconfig /displaydns** zeigt den Inhalt des DNS Cach in der alten Kommandozeile
 ```cmd
ipconfig /displaydns
``
ALternativ in der PowerShell
```powershell
Get-DnsClientCache
```
Weitere Parameter und Verwendung [Link zu MicrosoftDocs](https://docs.microsoft.com/en-us/powershell/module/dnsclient/get-dnsclientcache?view=windowsserver2022-ps)

- **ipconfig /flushdns** leert den DNS ClientAche in der alten Kommandozeile
  ```cmd
  ipconfig /flushdns
  ```
  Alternativ in der PowerShell
  ```powershell
  Clear-DnsClientCache
  ```
  Weitere Parameter und Verwendung [Link zu MicrosoftDocs](https://docs.microsoft.com/en-us/powershell/module/dnsclient/clear-dnsclientcache?view=windowsserver2022-ps)

- **ping** zum senden von ICMP Request
```cmd
ping 8.8.8.8
```
Alternativ in der PowerShell
```powershell
Test-Connection -Computername 8.8.8.8
```
Weitere Parameter und Verwendung [Link zu MicrosoftDocs](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/test-connection?view=powershell-5.1)
