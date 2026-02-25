# firewall_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of firewall profiles to disable
# Uses ansible.windows.win_firewall module
firewall_profiles_disable:
#  - profiles:
#      - trusted

# List of firewall profiles to enable
# Uses ansible.windows.win_firewall module
firewall_profiles_enable:
#  - profiles:
#      - domain
#      - private
#      - public

# List of firewall rules to disable
# Uses community.windows.win_firewall_rule module
firewall_rules_disable:
#  - name: Remote Desktop - User Mode (TCP-In)
#    description: >-
#      Inbound rule for the Remote Desktop service to allow RDP traffic. [TCP 3389]
#    group: '@FirewallAPI.dll,-28752'
#    localport: 3389
#    action: allow
#    direction: in
#    protocol: tcp
#    profiles:
#      - domain
#      - private
#      - public

# List of firewall rules to enable
# Uses community.windows.win_firewall_rule module
firewall_rules_enable:
#  - name: OpenSSH SSH Server (sshd)
#    description: Inbound rule for OpenSSH SSH Server (sshd)
#    group: OpenSSH Server
#    localport: 22
#    action: allow
#    direction: in
#    protocol: tcp
#    profiles:
#      - domain
#      - private
#      - public
</pre>

## License

GPLv3+
