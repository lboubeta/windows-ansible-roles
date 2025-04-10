# dsc_settings role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# DSC settings to apply with ansible.windows.win_dsc
# Set inject_facts_as_vars = False to avoid warnings
# Each setting requires: setting, resource_name, parameters
# Optional: reboot (true/false, defaults to false if omitted)
dsc_settings:
#  - setting: Create C:\Temp
#    resource_name: File
#    parameters:
#      DestinationPath: C:\Temp
#      Type: Directory
#      Ensure: Present
#
#  - setting: Enable User Account Control (UAC)
#    resource_name: Registry
#    parameters:
#      Key: HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System
#      ValueName: EnableLUA
#      ValueType: DWord
#      ValueData: 1
#      Ensure: Present
#    reboot: true
#
#  - setting: Set WER local crash dump folder
#    resource_name: Registry
#    parameters:
#      Key: HKLM:\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps
#      ValueName: DumpFolder
#      ValueType: ExpandString
#      ValueData: '%LOCALAPPDATA%\CrashDumps'
#      Ensure: Present
#
#  - setting: Set WER local crash dump count
#    resource_name: Registry
#    parameters:
#      Key: HKLM:\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps
#      ValueName: DumpCount
#      ValueType: DWord
#      ValueData: 10
#      Ensure: Present
#
#  - setting: Set WER local crash dump type
#    resource_name: Registry
#    parameters:
#      Key: HKLM:\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps
#      ValueName: DumpType
#      ValueType: DWord
#      ValueData: 1
#      Ensure: Present
#
#  - setting: Enable new network location wizard
#    resource_name: Registry
#    parameters:
#      Key: HKLM:\SYSTEM\CurrentControlSet\Control\Network
#      ValueName: NewNetworkWindowOff
#      Ensure: Absent

# Reboot after DSC changes
# Action depends on per-setting "reboot: true"
dsc_settings_reboot: true
</pre>

## License

GPLv3+
