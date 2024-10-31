# registry_settings role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Registry settings to apply with ansible.windows.win_regedit
registry_settings:
#  - setting: Enable User Access Control (UAC)
#    path: HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System
#    name: EnableLUA
#    type: DWord
#    data: 1
#    reboot: true
#
#  # NB. This would replace %SystemRoot%\System32; with C:\Windows\System32
#  # NB. The calling playbook must gather the needed facts for this to work
#  # For example:
#  # - name: Gather needed facts
#  #   ansible.windows.setup:
#  #     gather_subset:
#  #       - '!all'
#  #       - '!min'
#  #       - env
#  #   when: ansible_facts.env is not defined
#  #- setting: Add C:\Tools to system Path
#  #  path: HKLM:\SYSTEM\CurrentControlSet\Control\Session Manager\Environment
#  #  name: Path
#  #  type: ExpandString
#  #  data: "{{ ansible_facts.env.Path if 'C:\\Tools;' in ansible_facts.env.Path
#  #                                   else ansible_facts.env.Path + 'C:\\Tools;' }}"
#  #  reboot: true
#
#  - setting: Set system TEMP folder
#    path: HKLM:\SYSTEM\CurrentControlSet\Control\Session Manager\Environment
#    name: TEMP
#    type: ExpandString
#    data: '%SystemRoot%\TEMP'
#    reboot: true
#
#  - setting: Set system TMP folder
#    path: HKLM:\SYSTEM\CurrentControlSet\Control\Session Manager\Environment
#    name: TMP
#    type: ExpandString
#    data: '%SystemRoot%\TEMP'
#    reboot: true
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