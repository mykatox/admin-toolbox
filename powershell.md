# Powershell
- [introduction](https://learn.microsoft.com/en-us/powershell/scripting/overview?view=powershell-7.6)

# Sharepoint
- [connect sharepoint online](https://learn.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online)

# Client Administration
- [Admin Tasks](https://learn.microsoft.com/en-us/training/paths/maintain-system-administration-tasks-windows-powershell/)
- [computer info](https://learn.microsoft.com/en-us/training/modules/manage-settings-for-local-windows-machine-use-powershell-cmdlets/2-manage-windows-10])
- [permissions](https://learn.microsoft.com/en-us/training/modules/manage-settings-for-local-windows-machine-use-powershell-cmdlets/3-manage-permissions-powershell)
- [Management Module](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.management/?view=powershell-5.1)

# Powershell 7
- [migration from 5 -> 7](https://learn.microsoft.com/en-us/powershell/scripting/whats-new/migrating-from-windows-powershell-51-to-powershell-7?view=powershell-7.6)
- [ps7 Module compatibility](https://learn.microsoft.com/en-us/powershell/scripting/whats-new/module-compatibility?view=powershell-7.6)
- [install Powershell 7](https://learn.microsoft.com/de-de/powershell/scripting/install/install-powershell-on-windows?view=powershell-7.6)


# Windows debloating script
- [howtogeek article](https://www.howtogeek.com/the-de-bloating-powershell-command-i-run-on-every-windows-install/)
- [winutils script](https://github.com/christitustech/winutil)

# Event Log
`Get-EventLog -LogName Application -EntryType Error -Newest 20`  
`Get-EventLog -LogName Application -Newest 20 -InstanceId 1002 -source *hang*`  
`Get-EventLog -LogName System -EntryType Error -Newest 20`  
- [learn Microsoft](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.management/get-eventlog?view=powershell-5.1)



