# etc_hosts role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# /etc/hosts header to always apply (subject to etc_hosts_omit_entries)
# This default header matches the default Windows header used a long time
etc_hosts_header: |
  #  Copyright (c) 1993-2009 Microsoft Corp.
  #
  # This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
  #
  # This file contains the mappings of IP addresses to host names. Each
  # entry should be kept on an individual line. The IP address should
  # be placed in the first column followed by the corresponding host name.
  # The IP address and the host name should be separated by at least one
  # space.
  #
  # Additionally, comments (such as these) may be inserted on individual
  # lines or following the machine name denoted by a '#' symbol.
  #
  # For example:
  #
  #      102.54.94.97     rhino.acme.com          # source server
  #       38.25.63.10     x.acme.com              # x client host

  # localhost name resolution is handled within DNS itself.
  #	127.0.0.1       localhost
  #	::1             localhost

# Add entry for host itself based on Ansible facts
# This will use the first IP address found in system
# This should be disabled when not using static IP
etc_hosts_self_add: false

# Force domain name used in host self entry
# If unset defaults to ansible_facts.domain
# Required if ansible_facts.domain is empty
etc_hosts_self_domain:

# List of lines to add to /etc/hosts
# NB. Other entries will be removed
etc_hosts_entries:
#  - 192.168.122.1    gateway.example.com gateway
#  - 192.168.122.150  bastion.example.com bastion

# /etc/hosts entries to omit
# none - do not omit entries
# ipv4 - omit all IPv4 entries
# ipv6 - omit all IPv6 entries
etc_hosts_omit_entries: none
</pre>

## License

GPLv3+