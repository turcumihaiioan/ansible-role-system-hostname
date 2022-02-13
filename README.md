system_hostname
=========

This role allows you to use the community.general.hostname module to set a system's hostname.

Requirements
------------

ansible >= 2.10

Role Variables
--------------

```
system_hostname:
  name: ...
  use: ...
```

Dependencies
------------

None

Example Playbook
----------------

#### Set a hostname:
```
- hosts: servers
  vars:
    system_hostname:
      name: web01
  roles:
    - turcumihaiioan.system_hostname
```

#### Set a hostname specifying strategy:
```
- hosts: servers
  vars:
    system_hostname:
      name: web01
      use: systemd
  roles:
    - turcumihaiioan.system_hostname
```

License
-------

GPL-3.0-only

Author Information
------------------

Role created by Turcu Mihai Ioan
