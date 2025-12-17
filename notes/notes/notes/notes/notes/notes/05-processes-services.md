# Processes + Services

## Processes
- `Get-Process`
- `Get-Process | Sort-Object CPU -Descending | Select-Object -First 10`
- `Stop-Process -Id 1234 -Force`

## Services
- `Get-Service`
- `Get-Service | Where-Object {$_.Status -eq "Running"}`
- `Start-Service Spooler`
- `Stop-Service Spooler`
