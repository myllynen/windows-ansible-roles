# wsl_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable WSL
# Requires Windows Server 2022+
# Disabling WSL will uninstall all currently
# installed distributions and the WSL feature
# Set to null to leave the current setup untouched
wsl_configuration_enable: true

# Reboot after WSL install or uninstall
# NB. Reboot is mandatory to complete un/install
#     and later steps will fail before rebooting
wsl_configuration_reboot: true

# Update WSL during configuration
# NB. This task does not support check mode,
#     if enabled update is always attempted.
wsl_configuration_update: false

# List of distributions to install
# See wsl.exe --list --online for alternatives
wsl_configuration_distributions:
#  - FedoraLinux-42

# Remove distributions not listed above
wsl_configuration_distributions_exclusive: false

# Default WSL distribution
wsl_configuration_distribution_default:

# List of distributions to update
# NB. This task does not support check mode, so
#     if enabled an update is always attempted.
wsl_configuration_distributions_update: "{{ wsl_configuration_distributions }}"

# Update commands for each distribution variant
# Patterns are case-insensitive, first match will be used
wsl_configuration_distribution_update_commands:
  arch_like:
    patterns: ['*archlinux*']
    commands: ['pacman -Syyu --noconfirm']
  debian_like:
    patterns: ['*Debian*', '*kali*', '*Ubuntu*']
    commands: ['apt-get update', 'apt-get upgrade -y']
  redhat_like:
    patterns: ['*Alma*', '*CentOS*', '*Fedora*', '*Oracle*', '*podman*', '*RHEL*']
    commands: ['dnf update --refresh -y']
  suse_like:
    patterns: ['*SUSE*']
    commands: ['zypper update -y']
  default:
    patterns: ['*']
    commands: ['/bin/true']
</pre>

## License

GPLv3+
