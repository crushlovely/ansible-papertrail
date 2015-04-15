# Ansible role to install Sidekiq

[![Build Status](https://img.shields.io/circleci/project/crushlovely/ansible-sidekiq-upstart.svg?style=flat)](https://img.shields.io/circleci/project/crushlovely/ansible-sidekiq-upstart)
[![Current Version](http://img.shields.io/github/release/crushlovely/ansible-sidekiq-upstart.svg?style=flat)](https://galaxy.ansible.com/list#/roles/1180)

This Ansible role installs/updates Sidekiq.  It also copies a working Upstart script.

## Installation

``` bash
$ ansible-galaxy install crushlovely.sidekiq-upstart,v1.0.0
```

## Variables

``` yaml
app_name: test
app_path: /home/ubuntu/test
server_env: qa
app:
  process_name: "{{ app_name }}"
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
- hosts: localhost
  roles:
    - crushlovely.sidekiq-upstart
```

## Dependencies

None

## License

MIT