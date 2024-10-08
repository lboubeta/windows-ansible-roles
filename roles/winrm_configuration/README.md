# winrm_configuration role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable WinRM
winrm_configuration_enable: true

# WinRM service start mode: auto or delayed
winrm_configuration_start_mode: auto

# Enable Basic-over-HTTPS with self-signed cert
# if WinRM HTTPS listener is not yet configured
winrm_configuration_https_enable: true

# Optionally block WinRM HTTP port
winrm_configuration_http_block: true

# WinRM service configuration
# CBT is None, Relaxed, or Strict
winrm_configuration_service_config:
  AllowUnencrypted: false
  Auth:
    Basic: true
    Kerberos: true
    Negotiate: true
    Certificate: false
    CredSSP: false
    CbtHardeningLevel: Relaxed
  IPv4Filter: '*'
  IPv6Filter: '*'

# Firewall profiles to apply rules
winrm_configuration_firewall_profiles:
  - domain
  - private

# Optionally display current configuration
winrm_configuration_display_config: false
</pre>

## License

GPLv3+
