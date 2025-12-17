# Pipeline + Objects (the “PowerShell is different” part)

PowerShell pipes OBJECTS, not plain text.

## Inspect output
- `Get-Process | Get-Member`
- `Get-Service | Get-Member`

## Select properties
- `Get-Process | Select-Object Name, Id, CPU`
- `Get-Service | Select-Object Name, Status, StartType`

## Sort / Filter
- `Get-Process | Sort-Object CPU -Descending | Select-Object -First 10`
- `Get-Service | Where-Object {$_.Status -eq "Running"}`

## Format (for display)
- `Get-Process | Format-Table -AutoSize`
- `Get-Process | Format-List *`
