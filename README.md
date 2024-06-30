# Win_Registry_to_monitor
Registry keys to monitor for changer in Windows as they are known to be used by adversaries.
The purpose of this project is to gather info on important Registry keys that adversaries use for Defense evasion, Persistance ... on Windows systems. 
Using freely available info from: https://attack.mitre.org/, Sigma rules, Sysmon rules, various reports and hackers sites on hacking tactics that rely on Registry modification. 
If successful, a simple scan tool can be also developed based on this list that will check systems if they are protected and/or  possibly compromised like Loki IoC scanner.

Genral info:

https://attack.mitre.org/techniques/T1112/

https://github.com/SigmaHQ/sigma/tree/master/rules/windows/registry

https://github.com/Defenders-Guide/TheDefendersGuide/blob/main/Windows/Windows%20Registry/Highly%20Targeted%20Registry%20Keys.csv


## AMSI

HKLM:\SOFTWARE\Microsoft\AMSI\Providers\{2781761E-28E0-4109-99FE-B9D127C57AFE} (Defender)

HKCU\Software\Microsoft\Windows Script\Settings\AmsiEnable (https://ppn.snovvcrash.rocks/pentest/infrastructure/ad/av-edr-evasion/amsi-bypass)

## UAC

## SmartScreen

## AppLocker

## ATP

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows Advanced Threat Protection

## Microsoft antimalware:

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Microsoft Antimalware

## Microsoft Security center: 

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Security Center

## Microsoft Security manager: 

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\SecurityManager


# Defender:

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows Defender

## Real-time protection

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows Defender\real-time protection

## Exploit Guard

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows Defender\Windows Defender Exploit Guard


# Firewall:

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\WindowsFirewall

## Device guard: 

Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\DeviceGuard

## DMA security: 

Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\DmaSecurity

## Startup: 

HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run
HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\RunOnce
HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run
HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\RunOnce
Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders (Folders to start when user logs on)
HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\Windows\AppInit_DLLs (ists DLLs to be loaded into every process that loads user32.dll)
