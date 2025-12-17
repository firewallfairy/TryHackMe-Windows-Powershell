# Security / Forensics-ish basics

## Users / identity
- `whoami`
- `whoami /groups`
- `Get-LocalUser`
- `Get-LocalGroup`
- `Get-LocalGroupMember Administrators`

## Event logs
- `Get-WinEvent -ListLog * | Select-Object -First 20`
- `Get-WinEvent -LogName Security -MaxEvents 20`
- `Get-WinEvent -FilterHashtable @{LogName="Security"; Id=4624} -MaxEvents 10`

## Scheduled tasks
- `Get-ScheduledTask | Select-Object TaskName, State | Select-Object -First 30`

## Startup-ish spots (basic)
- `Get-CimInstance Win32_StartupCommand | Select-Object Name, Command, Location`
