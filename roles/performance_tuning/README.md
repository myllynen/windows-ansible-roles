# performance_tuning role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# NTFS Last Access Time updates
ntfs_last_access_time_update: false

# Page file configuration
# auto      - automatically managed
# disabled  - page file fully disabled
# size      - static page file size in MB
# system    - system managed page file size
page_file_size: auto
page_file_disk: C

# Reboot after page file change
page_file_reboot: true

# Power scheme configuration
# balanced          - balance between performance and energy use
# power_saver       - max energy savings at the cost of performance
# high_performance  - maximum performance with higher energy use
power_scheme: balanced
</pre>

## License

GPLv3+
