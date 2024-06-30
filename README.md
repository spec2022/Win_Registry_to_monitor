# Win_Registry_to_monitor
Registry keys to monitor for changer in Windows as they are known to be used by adversaries.
https://attack.mitre.org/techniques/T1112/
https://github.com/SigmaHQ/sigma/tree/master/rules/windows/registry


## AMSI
HKLM:\SOFTWARE\Microsoft\AMSI\Providers\{2781761E-28E0-4109-99FE-B9D127C57AFE} (Defender)
HKCU\Software\Microsoft\Windows Script\Settings\AmsiEnable (https://ppn.snovvcrash.rocks/pentest/infrastructure/ad/av-edr-evasion/amsi-bypass)

## UAC

## SmartScreen
