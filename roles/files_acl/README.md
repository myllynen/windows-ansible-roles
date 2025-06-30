# files_acl role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of ACLs to apply to files etc
# Uses ansible.windows.win_acl module
# Owner set with win_owner if defined
# Registers variable: acl_files
files_acl:
#  - path: C:\Temp\log.txt
#    #owner: BUILTIN\Administrator
#    user: testuser
#    type: deny
#    rights: Read,Write,Modify,FullControl,Delete
#    state: present

# List of ACLs inheritance rules to apply to paths
# Uses ansible.windows.win_acl_inheritance module
# Registers variable: acl_inheritance_files
files_acl_inheritance:
#  - path: C:\apache
#    state: present
#    reorganize: true
</pre>

## License

GPLv3+
