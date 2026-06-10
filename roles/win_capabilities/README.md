# win_capabilities role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Windows capabilities to remove
win_capabilities_remove:
#  - Language.Speech~~~en-US~0.0.1.0
#  - App.StepsRecorder
#  - AzureArcSetup
#  - Browser.InternetExplorer
#  - DirectX.Configuration.Database
#  - Language.Handwriting~~~en-US~0.0.1.0
#  - Language.OCR~~~en-US~0.0.1.0
#  - MathRecognizer
#  - Media.WindowsMediaPlayer
#  - Microsoft.Windows.MSPaint
#  - Microsoft.Windows.SnippingTool
#  - OneCoreUAP.OneSync
#  - VBSCRIPT
#  - XPS.Viewer
#  # Windows needs time after removing
#  # the corresponding Language.Speech
#  # to be able to remove this capability
#  - Language.TextToSpeech~~~en-US~0.0.1.0

# Ignore failures to remove unknown capabilities
win_capabilities_remove_ignore_unknown: true

# Windows capabilities to install
win_capabilities_install:
#  - OpenSSH.Client
#  - OpenSSH.Server
#  - name: Corp.Infra.Tools
#    source: D:\Sources
#    disable_windows_update: true

# Reboot if needed after changes
win_capabilities_reboot: true

# Empty/unset uses the default DISM log
win_capabilities_log_path:

# DISM logging level
# 0 - logs errors only
# 1 - logs errors and warnings
# 2 - logs errors, warnings, and information
# 3 - logs all of the previous plus debug output
win_capabilities_log_level: 1
</pre>

## License

GPLv3+
