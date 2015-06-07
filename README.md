# ansible-role-supervio

Ansible playbook to automate installing, upgrading and configuring VIO.

## Requirements

This role currently supports CentOS and Debian/Ubuntu distros and requires a valid installation of VMware's OVFTools.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    vio_config_json: "~/vio_config.json"

The full path to a file in which to place the VIO JSON configuration file template."

## Example playbook

```
---
- name:  Deploy OVA and create config.json for vio
  hosts: local
  roles:
    - vio
  vars_files:
    - /vars/uianswers.yml
```

## License

TBD

## Author Information

This role was created in 2015 by [Devin Nance / VMware](http://www.vmware.com/).
