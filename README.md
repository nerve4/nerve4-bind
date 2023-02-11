# bind - base

An Ansible role that installs bind to Rhel. More info about bind: [link](https://www.isc.org/bind/)


## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

The Role also use `community.general collection` module. To install it, use: `ansible-galaxy collection install community.general`. 


## Tasks descriptions

- main.yml - Run the OS check and run the relevant playbook
- rhel-install-bind.yml - Deploy bind on Rhel
- configure-bind.yml - Configure bind on the hosts
- configure-clients.yml - Configure clients


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-bind
```


## Maintainer Information
Lee | 2023