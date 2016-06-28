# Ansible Role: gems

[![Build Status](https://travis-ci.org/AttestationLegale/ansible-role-gems.svg?branch=master)](https://travis-ci.org/AttestationLegale/ansible-role-gems) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-gems-blue.svg)](https://galaxy.ansible.com/AttestationLegale/gems/)

The gems role allows you to install ruby gems.


## Requirements

None

## Role Variables

For a complete list of variables, see `default/main.yml`.

    gems_packages: []
    gems_group_packages: []
    gems_host_packages: []

## Dependencies

None

## Example Playbook

```yaml
---
  - hosts: all
    vars:
      - gem_packages:
        - name: inifile
        - name: net-ping
          state: absent
    roles:
      - gems
```

## License

MIT / BSD

## Author Information

This role was created in 2016 by [ALG](https://www.attestationlegale.fr)
