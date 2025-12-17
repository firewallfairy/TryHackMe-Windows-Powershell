# Networking

## IP / config
- `ipconfig`
- `Get-NetIPConfiguration`
- `Get-NetIPAddress`

## DNS
- `Resolve-DnsName tryhackme.com`

## Connections / ports
- `netstat -ano`
- `Get-NetTCPConnection | Select-Object LocalAddress,LocalPort,RemoteAddress,RemotePort,State,OwningProcess`
- `Test-NetConnection 8.8.8.8`
- `Test-NetConnection google.com -Port 443`

## Firewall (view)
- `Get-NetFirewallProfile`
- `Get-NetFirewallRule | Select-Object DisplayName, Enabled, Direction, Action | Select-Object -First 25`
