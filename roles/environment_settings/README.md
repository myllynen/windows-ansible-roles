# environment_settings role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Path environment settings to configure
# Each setting requires: scope, name, elements, state
# Optional: reboot (true/false, defaults to false if omitted)
environment_settings_paths:
#  # These are for connecting user only
#  - scope: user
#    name: CLASSPATH
#    elements: C:\Java
#    state: present
#  - scope: user
#    name: CLASSPATH
#    elements: C:\OldJava
#    state: absent
#
#  # These are for all users
#  - scope: machine
#    name: PATH
#    elements: C:\Tools\bin
#    state: present
#
#  # Reboot if updated and environment_settings_reboot is true
#  - scope: machine
#    name: PATH
#    elements:
#      - C:\Dangerous\bin
#      - C:\Migration\bin
#    state: absent
#    reboot: true

# Environment variable settings to configure
# Each setting requires: level, variables
# Optional: reboot (true/false, defaults to false if omitted)
environment_settings_variables:
#  # These are for connecting user only
#  - level: user
#    variables:
#      ThisIsRemoved: ''
#      SomeVariable: SomeValue
#
#  # These are for all users
#  - level: machine
#    variables:
#      TestVariable: Test value
#
#  # Reboot if updated and environment_settings_reboot is true
#  - level: machine
#    variables:
#      VIV: VeryImportantValue
#    reboot: true

# Reboot after environment setting changes
# Action depends on per-setting "reboot: true"
environment_settings_reboot: true
</pre>

## License

GPLv3+
