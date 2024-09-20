# rdp_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable RDP
rdp_configuration_enable: true

# Firewall profiles to apply rules
rdp_configuration_firewall_profiles:
  - domain
  - private

# Require authentication for RDP
rdp_configuration_authenticate: true
</pre>

## License

GPLv3+
