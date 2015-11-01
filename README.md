# consul-install

Installs [Hasicorp's Consul] (https://consulproject.io)



## Role Variables
```yml

---
consul:
  version: 0.5.2
  arch: amd64

install:
  dir : /usr/local/bin
  web_dir: /var/www/html/consul
  download_location: https://dl.bintray.com/mitchellh/consul

```


Example Playbook
----------------
```yml

---
- hosts: local
  sudo: true
  gather_facts: true

  roles:
    - marcelocorreia.consul-install

  vars_files:
    - ../vars/tardis.yml

```

License
-------

MIT

Author Information
------------------
Some useful stuff at:
  - [https://github.com/marcelocorreia](https://github.com/marcelocorreia)
  - [https://galaxy.ansible.com/list#/users/15516](https://galaxy.ansible.com/list#/users/15516)
  - [https://hub.docker.com/u/marcelocorreia/](https://hub.docker.com/u/marcelocorreia/)
  - Any issues, pull-request are welcome
