# Group policies
report als HTML Datei erstellen  
`gpresult /h c:\temp\gpreport.html`

report im terminal anzeigen  
`gpresult /r`

conflicting GPOs  
`gpresult /z`

als GUI anzeigen  
`rsop.msc`

for intune managed devices  
`mdmdiagnostictool.exe`


# Active Directory
[RSAT](https://learn.microsoft.com/de-de/troubleshoot/windows-server/system-management-components/remote-server-administration-tools)  
dcpromo, ldp, netdom, ntdsutil, repadmin, dcdiag, dsals, dsadd, dsdbutil, dsmgmt, dsmod, dsmove,
dsquery, dsrm, gpfixup, ksetup, nitest, nslookup, w32tm



# Tools
- [sysinternals](https://learn.microsoft.com/de-de/sysinternals/)  
- [powertoys](https://learn.microsoft.com/de-de/windows/powertoys/)  
- [NirSoft](https://www.nirsoft.net/)  
- Process Explorer
- [WhatIsHang](https://www.nirsoft.net/utils/what_is_hang.html)
- [ProcMon](https://learn.microsoft.com/de-de/sysinternals/downloads/procmon)
- resmon.exe - Ressourcenmonitor
- [USB Tree View](https://www.uwe-sieber.de/usbtreeview.html)
- TCPView (Sysinternals)

# Hardware
devmgmt.msc - Gerätemanager
[learn Hardware/driverres](https://learn.microsoft.com/de-de/windows-hardware/drivers/)  
 

# USB
- [learn USB](https://learn.microsoft.com/de-de/windows-hardware/drivers/usbcon/)  
- [MUTT](https://learn.microsoft.com/de-de/windows-hardware/drivers/usbcon/microsoft-usb-test-tool--mutt--devices)  
- [MUTT Tools](https://learn.microsoft.com/de-de/windows-hardware/drivers/usbcon/mutt-software-package)  
- [USB-Hardwareprüfer](https://learn.microsoft.com/de-de/windows-hardware/drivers/usbcon/how-to-retrieve-information-about-a-usb-device)

Energiesparmodus für USB Geräte im Geräte-Manager prüfen 
Energieoptionen - selektive USB-Energiesparen

USB-Serial Bridge, Gerätemanager COM-Port (Anschlusseinstelungen-Erweitert) - Wartezeit (latency Timer)

[Tool USBDeview](https://www.nirsoft.net/utils/usb_devices_view.html)

# Defender

- [defender ausschlüsse](https://learn.microsoft.com/de-de/defender-endpoint/configure-extension-file-exclusions-microsoft-defender-antivirus)
[ powershell](https://superuser.com/questions/1877991/how-can-i-add-a-disk-in-the-windows-defender-exclusion-list-without-having-to-at)
- [persistent exclusions](https://cloudbrothers.info/en/create-persistent-defender-av-exclusions-circumvent-defender-endpoint-detection/)

Powershell
`Add-MpPreference -ExclusionPath 'D:\'`



# Bitlocker
- [recovery key](https://aka.ms/aadrecoverykey)
- [exclude removable USB drives from automatic encryption](https://petervanderwoude.nl/post/excluding-removable-usb-drives-from-automatic-encryption/)
- [learn Microsoft](https://learn.microsoft.com/de-de/windows/security/operating-system-security/data-protection/bitlocker/configure?tabs=common)
- [exclusion with group policies](https://learn.microsoft.com/en-us/answers/questions/2186434/bitlocker-external-drive-exclusion-list-for-window)


# Intune
- [petervanderwoude](https://petervanderwoude.nl/)

# Config
## God Mode 
- folder with system settings 
- Desktop Shortcut `C:\Windows\explorer.exe shell:::{ED7BA470-8E54-465E-825C-99712043E01C}`  
- Rename folder to `GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}`  
[learn Microsoft](https://learn.microsoft.com/en-us/answers/questions/4140616/how-to-enable-god-mode-in-windows-11)
[article by kapilarya](https://www.kapilarya.com/how-do-you-enable-god-mode-in-windows-11)  

# Sentinel Hardware Dongle
- [Sentinel Admin Control Center](http://localhost:1947)

# Treiber
Treiber Reste finden und entfernen
1. CMD  
2. `set devmgr_show_nonpresent_devices=1`  
3. `start devmgmt.msc`  
4. Ansicht -> Ausgeblendete Geräte anzeigen  
5. ausgegraute Einträge -> Rechtsklick -> Gerät deinstallieren

