ECGALAXY soapui role
====================

Ansible role which installs SoapUI.

Requirements
------------

None.

Role Variables
--------------

- `soapui_version`: the version to download
- `soapui_url`: the URL from where to download the SH install script
- `soapui_role_working_dir`: the location on where to store temporary files
- `soapui_install_dir`: the location on where to install SoapUI
- `soapui_cleanup`: set to `true` (default) to clean up temporary files
- `soapui_uninstall`: set to `true` to uninstall

Dependencies
------------

This role depends on the following ECGALAXY roles:

- ecgalaxy.bootstrap
- ecgalaxy.common_packages
- ecgalaxy.java_openjdk

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.bootstrap
        - ecgalaxy.common_packages
        - ecgalaxy.java_openjdk
        - ecgalaxy.soapui

One-liner
---------

    bash <(curl -s https://code.europa.eu/-/snippets/1/raw/main/ansible-role.sh) ecgalaxy.soapui

See [ansible-role](https://code.europa.eu/-/snippets/1) for instructions.

Please verify the script integrity first.

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

[ECGALAXY](https://code.europa.eu/groups/ecgalaxy/-/wikis/home) team.
