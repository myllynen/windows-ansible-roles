# user_settings role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# For system-wide settings see registry_settings

# Some settings may apply only after relogin
user_settings_apply_to_logged_in_users: true

# User settings to apply with ansible.windows.win_regedit
user_settings_registry:
#  - setting: Minimize Visual Effects for Performance
#    path: HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\VisualEffects
#    name: VisualFXSetting
#    type: DWord
#    data: 2
#
#  - setting: Disable Taskbar Animations
#    path: HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Advanced
#    name: TaskbarAnimations
#    type: DWord
#    data: 0
</pre>

## License

GPLv3+
