HASS Ansible role
==================

Role to manage HASS.

Requirements
------------

No requirements

Role Variables
--------------

- `hass__install` For install only (default: False)
- `hass__configure` For configuration  (default: False)
- `hass__install_packaged_docker` to use packaged docker (default: True)
- `hass__data_dir` to change default install path (default: undefined)

### nginx sidecars configs

- `hass__zigbee_sidecar` For installing a nginx service as a sidecar for Zigbee2mqtt (default: False)
- `hass__hostname` used by proxy nginx conf (if any). (default: undefined)
- `hass__zigbee_hostname` used by proxy nginx conf (if any) for zigbee. (default: undefined)
- `hass__use_ssl` set to true if proxy use SSL (default: undefined)
- `hass__zigbee_use_ssl` set to true if proxy use SSL on zigbee (default: undefined)
- `hass__ssl_cert` path to cert file (default: undefined)
- `hass__zigbee_ssl_cert` path to zigbee cert file (default: undefined)
- `hass__ssl_key` path to key file (default: undefined)
- `hass__zigbee_ssl_key` path to zigbee key file (default: undefined)

Dependencies
------------

None

Example Playbooks
-----------------

License
-------

GPL v3

Author Information
------------------

François TOURDE