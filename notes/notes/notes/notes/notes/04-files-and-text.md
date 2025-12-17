# Files + Text

## Reading files
- `Get-Content .\file.txt`
- `Get-Content .\file.txt -Tail 20`

## Searching text
- `Select-String -Path .\file.txt -Pattern "password"`
- `Select-String -Path .\*.log -Pattern "error"`

## Create / copy / move / delete
- `New-Item -ItemType File -Path .\test.txt`
- `Copy-Item .\a.txt .\b.txt`
- `Move-Item .\b.txt .\archive\`
- `Remove-Item .\test.txt`

## Recursion (grab everything)
- `Get-ChildItem -Recurse -Force`
