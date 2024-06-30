# Win_Registry_to_monitor
Registry keys to monitor for changer in Windows as they are known to be used by adversaries.
The purpose of this project is to gather info on important Registry keys that adversaries use for Defense evasion, Persistance ... on Windows systems. 
Using freely available info from: https://attack.mitre.org/, Sigma rules, Sysmon rules, various reports and hackers sites on hacking tactics that rely on Registry modification. 
If successful, a simple scan tool can be also developed based on this list that will check systems if they are protected and/or  possibly compromised like Loki IoC scanner.

Genral info:
https://attack.mitre.org/techniques/T1112/

https://github.com/SigmaHQ/sigma/tree/master/rules/windows/registry


## AMSI
HKLM:\SOFTWARE\Microsoft\AMSI\Providers\{2781761E-28E0-4109-99FE-B9D127C57AFE} (Defender)
HKCU\Software\Microsoft\Windows Script\Settings\AmsiEnable (https://ppn.snovvcrash.rocks/pentest/infrastructure/ad/av-edr-evasion/amsi-bypass)

## UAC

## SmartScreen
