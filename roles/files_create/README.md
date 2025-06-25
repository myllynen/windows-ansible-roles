# files_create role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of directories and files to create
# Uses ansible.windows.win_file module
# Owner set with win_owner if defined
# Registers variables:
# create_directories, create_files
files_create:
#  - state: directory
#    path: C:\Tools
#    #owner: BUILTIN\Administrators
#    #recurse: true
#  - state: file
#    path: C:\Tools\log.txt
#    #owner: S-1-5-21-...-1000
</pre>

## License

GPLv3+
