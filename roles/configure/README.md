Ansible Role Template
=========



This is an Ansible role to install and configure configure.

Include more information about configure in this section.

Requirements
------------
These platforms are supported:
- Ubuntu 20.04
- Debian 11
- EL 8 (Tested on Rocky Linux 8)

<!--
- List hardware requirements here  
-->

Role Variables
----------

The variables for this role are VERY insecure by default. Please change them to something more secure if you want to use this role. This role is meant for testing purposes only.

You can view the default variables in [defaults/main.yml](./defaults/main.yml).

Variable | Default | Description
--- | --- | ---

Dependencies
------------
<!-- List dependencies on other roles or criteria -->
None

Example Playbook
----------------

```yaml
- name: Use diademiemi.configure role
  hosts: "{{ target | default('configure') }}"
  roles:
    - role: "diademiemi.configure"
      tags: ['diademiemi', 'configure', 'setup']    ```

```

License
-------

MIT

Author Information
------------------

- diademiemi (@diademiemi)

Role Testing
------------

This repository comes with Molecule that run in Podman on the supported platforms.
Install Molecule by running

```bash
pip3 install -r requirements.txt
```

Run the tests with

```bash
molecule test
```

These tests are automatically ran by GitHub Actions on push. If the tests are successful, the role is automatically published to Ansible Galaxy.

