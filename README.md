ansible-role-vio
=========

An ansible role to deploy VIO ova, deploy VIO Cluster. This role also
creates the floating ip network. Addtionally this role will do a quick
validation of the VIO environment by creating a demo project, create or
add a demo user, deploy a heat stack into the newly created project.

The heat stack consists of networks, security groups, instances and a
user_data bash script to partition and mount a cinder volume.


Requirements
------------

* A vsphere and NSX environments for VIO.
* Ovftool

Role Variables
--------------

* vio_ova_path - full path to the location for the VIO ova
* vio_ova - Name of the VIO ova being used
* ovf_tool_path - path to the ovftool


Example Playbook
----------------
```yaml
- name:  VIO Deployment
  hosts: local
  connection: local
  roles:
    - vio
```

License
-------
Copyright 2015 VMware, Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may
not use this file except in compliance with the License. You may obtain
a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Author Information
------------------
VMware