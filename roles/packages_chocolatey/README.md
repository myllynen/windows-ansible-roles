# packages_chocolatey role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Parameters for Chocolatey installation
packages_chocolatey_update: true
packages_chocolatey_package_params:
packages_chocolatey_bootstrap_script:
packages_chocolatey_validate_certs: true

# Parameters to apply with win_chocolatey_source
packages_chocolatey_source:
#  - name: chocolatey
#    state: absent
#
#  - name: intranet repo
#    state: present
#    source: http://example.com/choco

# Parameters for Chocolatey configuration and features
# Items with value or state present/absent are set with
# win_chocolatey_config, rest with win_chocolatey_feature
# See https://docs.chocolatey.org/en-us/configuration/
packages_chocolatey_settings:
#  - name: cacheLocation
#    state: present
#    value: C:\Temp\choco
#
#  - name: checksumFiles
#    state: enabled
#
#  - name: logWithoutColor
#    state: enabled
#
#  - name: webRequestTimeoutSeconds
#    state: present
#    value: 10

# Parameters for package operations
packages_chocolatey_install_allow_prerelease: false
packages_chocolatey_install_ignore_dependencies: false
packages_chocolater_update_packages: true
packages_chocolatey_remove_deps: false

# Chocolatey packages to install
packages_chocolatey_install:
#  - git
#  - less
#  - nano
#  - vim

# Chocolatey packages to remove
packages_chocolatey_remove:
#  - emacs
</pre>

## License

GPLv3+
