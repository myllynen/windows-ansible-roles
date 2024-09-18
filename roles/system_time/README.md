# system_time role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
system_time_ntp_servers:
  - time.windows.com

system_time_timezone: UTC

# Reboot after timezone change
system_time_timezone_reboot: true
</pre>

## License

GPLv3+
