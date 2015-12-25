# terraform-install

Installs [Hasicorp's Terraform](https://terraform.io)



## Role Variables
```yml

---
terraform:
  version: 0.6.8
  arch: amd64

install:
  dir : /usr/local/bin
  download_location: https://releases.hashicorp.com/terraform/

```


Example Playbook
----------------
```yml

---
- hosts: local
  sudo: true
  gather_facts: true

  roles:
    - marcelocorreia.terraform-install

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
