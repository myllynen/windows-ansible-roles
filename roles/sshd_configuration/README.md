# sshd_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable sshd
sshd_configuration_enable: true

# Install OpenSSH.Server capability if needed
# Skipping this will speedup the role a little
# if sshd is already installed but the role is
# going to fail in case sshd is not installed.
# This is not needed with Windows Server 2025.
sshd_configuration_install: false

# Default shell for sshd, this must be kept in
# sync with ansible_shell_type to avoid errors
# NB. Needs an absolute path
# For cmd.exe the path is: C:\Windows\System32\cmd.exe
# For PowerShell must use: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
sshd_configuration_shell:

# Administrators SSH keys to add/remove
sshd_configuration_admins_keys:
#  absent:
#    - ssh-rsa ...
#  present:
#    - ssh-ed25519 ...

# sshd service start mode: auto or delayed
sshd_configuration_start_mode: auto

# Firewall profiles to apply rules
sshd_configuration_firewall_profiles:
  - domain
  - private
  - public

# Enable sshd_config validatiion using a copy if
# the file is about to be updated. Recommended.
sshd_configuration_config_validate: true

# sshd configuration file template to use
# This is mutually exclusive with the options below
# Role provided alternatives:
# * default_config - OpenSSH.Server 0.0.1.0 default
sshd_configuration_config_file:

# These options will be explicitly set in sshd_config,
# no other options will be left in place after update.
# The example set below matches OpenSSH.Server 0.0.1.0
sshd_configuration_options:
#  AuthorizedKeysFile: .ssh/authorized_keys
#  Subsystem: sftp sftp-server.exe
#  AllowGroups: administrators "openssh users"
#  Match Group administrators:
#    - AuthorizedKeysFile __PROGRAMDATA__/ssh/administrators_authorized_keys
</pre>

## License

GPLv3+