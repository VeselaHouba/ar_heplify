# Ansible role to install and start HepLify

Ansible role for HepLify (https://github.com/sipcapture/heplify)

## Tasks
### Variables:
- heplify_version: 1.62
- heplify_path: /opt/heplify
- heplify_interface: any
- heplify_types: af_packet
- heplify_modes: SIP
- heplify_hep_server: 127.0.0.1:9060
- heplify_id: 001


## Requirements
- Tested with vagrant box (Debian 8 / 9)
- Ansible 2.7.4

## Start to play
```
service heplify start
```

## Ansible Galaxy
https://galaxy.ansible.com/mickaelh51/ar_heplify
```
ansible-galaxy install mickaelh51.ar_heplify
```

## Enhancements
