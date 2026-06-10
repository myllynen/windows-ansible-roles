# win_features role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# See also win_capabilities and win_optional_features

# Windows features to remove
win_features_remove:
#  - System-DataArchiver
#  - Telnet-Client
#  - WindowsAdminCenterSetup
#  - Wireless-Networking

# Ignore failures to remove unknown features
win_features_remove_ignore_unknown: true

# Windows features to install
win_features_install:
#  - WoW64-Support
#  - name: Web-Server
#    source: D:\Sources
#    include_sub_features: true
#    include_management_tools: true

# Reboot if needed after changes
win_features_reboot: true
</pre>

## License

GPLv3+
