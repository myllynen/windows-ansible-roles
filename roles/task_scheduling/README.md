# task_scheduling role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# List of scheduled tasks to remove
# Uses community.windows.win_scheduled_task module
task_scheduling_remove:
#  - Incorrect task
#  - Obsoleted task

# List of scheduled tasks to create/enable/disable
# Uses community.windows.win_scheduled_task module
task_scheduling_create:
#  - name: Report system info
#    description: Daily system info update
#    enabled: true
#    actions:
#      - path: cmd.exe
#        arguments: /c systeminfo.exe > \Windows\Temp\systeminfo.txt
#    triggers:
#      - type: daily
#        start_boundary: '00:00:00'
#    username: SYSTEM
</pre>

## License

GPLv3+
