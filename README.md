# ansible-role-vio

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

# License and Copyright
 
Copyright 2015 VMware, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

## Author Information

This role was created in 2015 by [Devin Nance / VMware](http://www.vmware.com/).
