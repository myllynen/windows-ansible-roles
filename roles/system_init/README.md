# system_init role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Perform minor cleanups after system
# initial installation. See the tasks
# for details. Using this role is by
# no means mandatory or required.

# System initialization file
system_init_file: C:\Windows\init_info_system.txt

# System initialization message
system_init_msg_file: "This system was initialized by system_init on {{ '%Y-%m-%d %H:%M:%S %Z' | strftime }}.\r\n"
system_init_msg_log: "{{ system_init_msg_file }}"

# Actions to take after initialization
# reboot - reboot after initialization
# syslog - write message to system log
system_init_final_actions:
  - reboot
  - syslog
</pre>

## License

GPLv3+
