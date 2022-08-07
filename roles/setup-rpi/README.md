# setup-rpi
Ansible role to setup Raspberry Pi.

command: ansible-playbook -i <host_file> setup_rpi.yml

Sample setup_rpi.yml
```yaml
---
- hosts: rpi
  remote_user: pi
  become: yes
  become_method: sudo
       
  roles:
    - setup-rpi
```

