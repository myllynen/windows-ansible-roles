# service_recovery role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
service_recovery_options:
  - name: SNMPTRAP
    actions:
      - delay_ms: 30000
        type: restart
      - delay_ms: 30000
        type: restart
      - delay_ms: 60000
        type: reboot
</pre>

## License

GPLv3+
