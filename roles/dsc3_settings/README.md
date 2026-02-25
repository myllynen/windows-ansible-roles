# dsc3_settings role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# DSC3 settings to apply with ansible.windows.dsc3
# Each setting requires: setting and config or config_file
# Optional: parameters, trace_level, remote_config_file,
#           reboot (true/false, defaults to false if omitted)
dsc3_settings:
#  - setting: Install .NET
#    config:
#      resources:
#        - name: Install .NET Framework
#          type: Microsoft.WinGet/Package
#          properties:
#            id: Microsoft.DotNet.Framework.DeveloperPack_4
#            source: winget
#    reboot: true

# Reboot after DSC3 changes
# Action depends on per-setting "reboot: true"
dsc3_settings_reboot: true
</pre>

## License

GPLv3+
