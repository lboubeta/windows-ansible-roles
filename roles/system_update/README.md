# system_update role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Retry attempts and delay between retries
# for applying updates in case of failures
system_update_retry_count: 3
system_update_retry_delay: 30

# Parameters for win_updates
system_update_categories: '*'
system_update_accept_list: []
system_update_reject_list: []
system_update_skip_optional: true
system_update_state: installed

# Display update results
system_update_display_results: true

# Reboot if needed after updates
system_update_reboot: true
system_update_reboot_timeout: 1200

# Compile all installed assemblies
# This will happen only after updates
system_update_compile_assemblies: true

# Trigger compilation only when updates with
# the following description were part of the
# installed updates. Use '.*' for everything.
system_update_compile_filter: Cumulative Update
</pre>

## License

GPLv3+
