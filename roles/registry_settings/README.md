# registry_settings role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Registry settings to apply with ansible.windows.win_regedit
registry_settings:
#  - setting: Allow full admin privileges for local admins over WinRM
#    path: HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System
#    name: LocalAccountTokenFilterPolicy
#    type: DWord
#    data: 1
#
#  - setting: Enable User Account Control (UAC)
#    path: HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System
#    name: EnableLUA
#    type: DWord
#    data: 1
#    reboot: true
#
#  - setting: Set WER local crash dump folder
#    path: HKLM:\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps
#    name: DumpFolder
#    type: ExpandString
#    data: '%LOCALAPPDATA%\CrashDumps'
#
#  - setting: Set WER local crash dump count
#    path: HKLM:\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps
#    name: DumpCount
#    type: DWord
#    data: 10
#
#  - setting: Set WER local crash dump type
#    path: HKLM:\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps
#    name: DumpType
#    type: DWord
#    data: 1
#
#  - setting: Enable new network location wizard
#    path: HKLM:\SYSTEM\CurrentControlSet\Control\Network\NewNetworkWindowOff
#    state: absent

# Reboot after registry changes
# Action depends on per-setting "reboot: true"
registry_settings_reboot: true
</pre>

## License

GPLv3+
