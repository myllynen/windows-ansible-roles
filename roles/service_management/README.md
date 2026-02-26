# service_management role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Ignore missing services to avoid errors
service_management_ignore_missing: false

# List of services to remove/disable/stop/pause
# Required: name and either state or start_mode
# Uses ansible.windows.win_service module
service_management_disable:
#  - name: dev service
#    state: absent
#  - name: WSearch
#    start_mode: disabled
#    state: stopped
#  - name: WbioSrvc
#    start_mode: disabled
#    state: stopped

# List of services to create/configure/enable/start/restart
# Required: name and at least either state or start_mode
# Optional: ansible.windows.win_service parameters and
# restart_configured to restart after config changes
# Uses ansible.windows.win_service module
service_management_enable:
#  - name: new test service
#    start_mode: manual
#    state: stopped
#    path: C:\Temp\test.exe
#  - name: sshd
#    start_mode: auto
#    state: started
#  - name: wuauserv
#    start_mode: auto
#    state: started
#  - name: SNMPTrap
#    failure_actions:
#      - delay_ms: 10000
#        type: restart
#      - delay_ms: 20000
#        type: restart
#      - delay_ms: 30000
#        type: reboot
#    failure_reboot_msg: Rebooting after SNMPTrap service failure
#    failure_reset_period_sec: '0xFFFFFFFF'
#    restart_configured: true
</pre>

## License

GPLv3+
