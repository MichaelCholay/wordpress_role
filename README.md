wordpress_role
=========

Role to install wordpress (and mariadb) into docker containers.

Requirements
------------

A pre-requisite is to have docker on hosts. If necessary, it is possible to obtain docker with the michaelcholay.docker_role role available on Ansible galaxy with the command :
```bash
ansible-galaxy install michaelcholay.docker_role
```

Role Variables
--------------

Description of the settable variables for this role:
- mysql_port: host port (mapped with port 3306 of the container)
- mysql_root_password: password of root user
- mysql_db: name of the MySQL database
- mysql_user: name of MySQL user
- mysql_password: paswword of the MySQL user

Dependencies
------------

See Requirements section.

Example Playbook
----------------

```yml
---
- hosts: localhost
  remote_user: root
  roles:
    - wordpress_role
```

License
-------

BSD
