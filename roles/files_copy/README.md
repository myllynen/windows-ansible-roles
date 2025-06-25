# files_copy role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of files and directories to copy
# Uses ansible.windows.win_copy module
# Owner set with win_owner if defined
# Registers variable: copy_files
files_copy:
#  - src: /local/src/test.file
#    dest: C:\Temp\test.file
#    #owner: BUILTIN\Administrators

# List of templates to render
# Uses ansible.windows.win_template
# Owner set with win_owner if defined
# Registers variable: copy_templates
files_copy_templates:
#  - src: settings.conf.j2
#    dest: C:\Tools\settings.conf
#    #owner: S-1-5-21-...-1000
</pre>

## License

GPLv3+
