# hashicorp-pack

This role only install Hashicorp apps, defaults to /usr/local/bin.

It does not configure or push any templates. Boring but useful.

## Variables

```yml
hashicorp:
  apps:
    - name: nomad
      state: absent
      version: 0.2.3
    - name: vault
      state: absent
      version: 0.4.0
    - name: otto
      state: absent
      version: 0.2.0
    - name: packer
      state: absent
      version: 0.8.6
    - name: terraform
      state: absent
      version: 0.6.10
    - name: consul
      state: absent
      version: 0.6.3
    - name: consul-template
      state: absent
      version: 0.12.2
```

> Note: it does not remove the packages as yet, for the moment you can declare 
> as above or simply just add entries the you need you state=present. Removal
feature will be add soon. 
 

