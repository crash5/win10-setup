# Windows 10 First Steps


## Key Combinations

| Key | Description |
|-----|-------------|
| Win + Pause | Display the System Properties |


## General

- Disable memory compression PS:  Disable-MMAgent -mc
- Disable hibernation CMD: powercfg -h off
- Enable PS script for actual process: Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
- Hide lockscreen: gpedit > Administrative Templates > Control Panel > Personalization > Do not display the lock screen: Enabled
- Run PS script method CMD: if not exist success.log cmd /c powershell.exe -executionpolicy bypass our.ps1 > success.log
- Add QuickLaunch toolbar: %UserProfile%\AppData\Roaming\Microsoft\Internet Explorer\Quick Launch

## App remove

- Package List PS: Get-AppxPackage | Select Name, PackageFullName
- Remove package: Get-AppxPackage -allusers <PackageFullName> | Remove-AppxPackage
