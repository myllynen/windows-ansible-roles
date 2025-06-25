# files_get role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of files to get over network
# Uses ansible.windows.win_get_url
# Owner set with win_owner if defined
# Registers variable: get_files
files_get:
#  - url: https://server.example.com/data.zip
#    url_username: admin
#    url_password: admin123
#    url_timeout: 5
#    validate_certs: false
#    use_proxy: false
#    dest: C:\Temp\data.zip
#    #owner: S-1-5-21-...-1000

# Value for no_log parameter when getting
# files and using passwords, unset otherwise
files_get_no_log: true
</pre>

## License

GPLv3+
