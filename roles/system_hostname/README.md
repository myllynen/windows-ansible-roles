# system_hostname role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# System hostname to be configured in the system
#
# Should be short name (not FQDN) and valid for DNS
system_hostname: "{{ ansible_facts.hostname | upper }}"

# Reboot after system hostname change
system_hostname_reboot: true
</pre>

## License

GPLv3+
