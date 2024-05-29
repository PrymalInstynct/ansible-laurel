Ansible-Laurel
=========

Ansible Role to Deploy [Laurel Audit](https://github.com/threathunters-io/laurel) onto Red Hat or Debian based systems

Requirements
------------

ansible-core >= 2.10

Role Variables
--------------

Variables for this role are OS Family Dependent and can be found in the `vars` directory

```yaml
---
audisp_plugins_dir: /etc/audit/plugins.d/
selinux_enabled: true
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
---
- name: Install and Configure Laurel
  hosts: agents
  become: true
  roles:
    - PrymalInstynct.ansible_laurel
```

License
-------

GPLv3

Author Information
------------------

[Chad Zimmerman](https://github.com/PrymalInstynct)
