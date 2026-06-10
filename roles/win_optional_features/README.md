# win_optional_features role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Windows optional features to remove
win_optional_features_remove:
#  - Internet-Explorer-Optional-amd64
#  - WindowsMediaPlayer
#  - MediaPlayback
#  #- Microsoft-RemoteDesktopConnection
#  # NB. This typically fails to uninstall
#  #- Microsoft-Windows-Printing-PremiumTools
#  - Printing-Client
#  - Printing-Client-Gui
#  - Printing-PrintToPDFServices-Features
#  - Printing-XPSServices-Features
#  - SearchEngine-Client-Package
#  - Server-Drivers-Printers
#  - Server-Gui-Mgmt
#  - SmbDirect
#  - TelnetClient
#  - WindowsServerBackupSnapin
#  - WorkFolders-Client
#  - Xps-Foundation-Xps-Viewer

# Ignore failures to remove unknown optional features
win_optional_features_remove_ignore_unknown: true

# Windows optional features to install
win_optional_features_install:
#  - ServerCore-WOW64
#  - Windows-Defender
#  - Containers
#  - VirtualMachinePlatform
#  - Microsoft-Windows-Subsystem-Linux
#  - name: IIS-WebServer
#    source: D:\Sources
#    include_parent: true

# Reboot if needed after changes
win_optional_features_reboot: true
</pre>

## License

GPLv3+
