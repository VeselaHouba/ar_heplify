# Ansible Role: HepLify

[![Build Status](https://travis-ci.org/VeselaHouba/ansible-role-heplify.svg?branch=master)](https://travis-ci.org/VeselaHouba/ansible-role-heplify)

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
- Tested with molecule on Debian 8,9,10 and Ubuntu 14.04,16.04,18.04,20.04
- Ansible 2.7.4

## Start to play
```
service heplify start
```

## Ansible Galaxy
https://galaxy.ansible.com/veselahouba/ar_heplify
```
ansible-galaxy install veselahouba.heplify
```

## Credits
based on https://github.com/Mickaelh51/ar_heplify
