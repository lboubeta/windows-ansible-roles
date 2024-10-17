# system_locale role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# NB. Configuring keyboard for Welcome Screen is notoriously difficult, this
# role may or may not work reliably for that depending on the Windows version

# https://docs.microsoft.com/windows/win32/intl/table-of-geographical-locations
system_locale_location: 244

system_locale_system: en-US
system_locale_ui: en-US
system_locale_user: en-US
# Either a locale name (en-US, fi-FI, etc) or a hex code pair (0409:0000040B)
system_locale_input: en-US

# Force updating Welcome screen settings even if locale config was not changed
system_locale_welcome_screen_update_always: false

# Reboot after locale changes
system_locale_reboot: true
</pre>

## License

GPLv3+
