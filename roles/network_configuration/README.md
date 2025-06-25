# network_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable IPv6
network_configuration_ipv6_enable: true

# Enable or disable LMHOSTS lookup
network_configuration_lmhosts_enable: true

# Enable or disable NetBIOS
network_configuration_netbios_enable: true

# Reboot after IPv6/NetBIOS changes
network_configuration_reboot: true

# Static route configuration
# Each setting requires: destination, state
# When state is present also required: gateway, metric
network_configuration_routes:
#  - destination: 192.168.123.123/32
#    gateway: 192.168.1.1
#    metric: 1
#    state: present
#  - destination: 192.168.123.231/32
#    state: absent
</pre>

## License

GPLv3+
