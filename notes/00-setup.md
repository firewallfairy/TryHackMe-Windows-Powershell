# Setup / Basics

## Useful defaults
- `Get-ExecutionPolicy`
- `Set-ExecutionPolicy -Scope CurrentUser RemoteSigned`

## Profiles
- `$PROFILE`
- `Test-Path $PROFILE`
- `New-Item -ItemType File -Path $PROFILE -Force`

## Aliases
- `Get-Alias`
- `Get-Alias ls`
- `Set-Alias ll Get-ChildItem`
