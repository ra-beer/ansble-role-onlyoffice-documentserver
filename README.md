onlyoffice-documentserver
=========

Install a onlyoffice-documentserver.
Useable with and without https.

Requirements
------------

only tested on:
Ubuntu 20.04
nginx
postgresql
rabbitmq

root-access

Role Variables
--------------

onlyoffice_group: onlyoffice
onlyoffice_user: onlyoffice
onlyoffice_port_number: 80
db_name: onlyoffice
db_user: onlyoffice
# db_pwd: set this var at runtime for more secrurity
https: "yes"
email: "your@email.de"
domain: "your-domain.de"

Example Playbook
----------------

```yaml
---
- name: Server set up
  hosts: all
  roles:
    - name: onlyoffice
      role: onlyoffice
```

License
-------

MIT

Author Information
------------------

ra-rau
