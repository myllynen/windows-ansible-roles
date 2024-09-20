# performance_tuning role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Disable NTFS Last Access Time Stamp updates
ntfs_disable_last_access_time: true

# Page file size configuration
# auto - automatically managed
# disabled - page file disabled
# size - static page file size in MB
page_file_size: auto
page_file_disk: C

# Reboot after page file change
page_file_reboot: true
</pre>

## License

GPLv3+
