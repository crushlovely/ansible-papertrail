# Ansible role to install and Configure Papertrail

[![Build Status](https://circleci.com/gh/crushlovely/ansible-papertrail.svg?style=shield)](https://github.com/crushlovely/ansible-papertrail)
[![Current Version](http://img.shields.io/github/release/crushlovely/ansible-papertrail.svg?style=flat)](https://galaxy.ansible.com/list#/users/3804)

This Ansible role installs and configures Papertrail.

## Installation

``` bash
$ ansible-galaxy install crushlovely.papertrail,v1.0.0
```

## Variables

``` yaml
app_name: test
app_path: /home/ubuntu/test
server_env: qa
papertrail:
  host: app2.stuff.papertrail.com
  port: 12345
  log: "{{ app_path }}/{{ app_name }}.log"
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
- hosts: localhost
  roles:
    - crushlovely.papertrail
```

## Dependencies

None

## License

MIT