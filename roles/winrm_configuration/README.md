# winrm_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable WinRM
winrm_configuration_enable: true

# By default Basic / HTTPS connections
# will be enabled using a self-signed
# certificate in case the winrm HTTPS
# listener has not been configured yet.
# Disable this to skip configuring winrm
winrm_configuration_https_enable: true

# Optionally ensure WinRM HTTP port is blocked
winrm_configuration_http_block: true

# winrm service start mode: auto or delayed
winrm_configuration_start_mode: auto

# Firewall profiles to apply rules
winrm_configuration_firewall_profiles:
  - domain
  - private

# Optionally display current configuration
winrm_configuration_display_config: false
</pre>

## License

GPLv3+
