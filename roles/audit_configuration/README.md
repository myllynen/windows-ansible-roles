# audit_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of system-wide audit policy settings to apply
# Uses ansible.windows.win_audit_policy_system module
audit_configuration_system_policies:
#  - category: Account Logon
#    audit_type:
#      - success
#      - failure
#  - subcategory: File System
#    audit_type:
#      - failure

# Ignore missing rules on remove to avoid errors
audit_configuration_ignore_missing: false

# List of audit rules to remove
# Uses ansible.windows.win_audit_rule module
audit_configuration_rules_remove:
#  - path: C:\Windows\Temp
#    user: BUILTIN\Users

# List of audit rules to create
# Uses ansible.windows.win_audit_rule module
audit_configuration_rules_create:
#  - path: HKLM:\Software
#    user: BUILTIN\Users
#    rights:
#      - delete
#    audit_flags:
#      - success
</pre>

## License

GPLv3+
