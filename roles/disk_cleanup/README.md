# disk_cleanup role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Remove older versions of Windows Update files
disk_cleanup_windows_update_files: false

# Also remove files needed to uninstall updates
disk_cleanup_windows_update_reset: false

# Windows event logs clearing
disk_cleanup_event_logs: false
</pre>

## License

GPLv3+
