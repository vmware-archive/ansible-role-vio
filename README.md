ansible-role-vio
=========

An ansible role to deploy VIO

Requirements
------------

A vsphere and NSX environments for VIO. VIO ova

Role Variables
--------------

vio_ova_path - full path to the location for the VIO ova
vio_ova - Name of the VIO ova being used
ovf_tool_path - path to the ovftool


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


Author Information
------------------
