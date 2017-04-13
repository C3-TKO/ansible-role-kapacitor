# ansible-role-kapacitor

This is an Ansible role for installing and configuring kapacitor on a rapsberry pi. This role is meant to be used within my my-pi-setups repository https://github.com/C3-TKO/my-pi-setups.


## Requirements

- Tested on Ansible 2.2.10
- Tested on Ubuntu 16.04 (xenial), but it should work on any modern Debian based system.

## Dependencies

This role expects that the host machine has already ufw and python setup - You can use my common role from the main repository to setup ufw and python 
https://github.com/C3-TKO/my-pi-setups/tree/master/ansible/roles/common

## Example playbook

You can include this role in your playbook like this:

    ---
    - name: Install kapacitor
      hosts: kapacitor
      become: yes
      become_method: sudo

    roles:
      - kapacitor

## Licence

MIT

## Feedback? Found a bug? Requests?

Let me have it! https://github.com/C3-TKO/ansible-role-kapacitor/issues
