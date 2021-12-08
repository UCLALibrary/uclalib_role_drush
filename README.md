# UCLALib Ansible Role: Drush

Ansible role to install Drush (and Composer).

**This role is no longer maintaned and the repo is archived**

## Requirements

PHP 5.4.5 or later, to support Drush 8.

## Variables

See `defaults/main.yml`.  The only variable which should be changed is `drush_version`, which should be the latest build of Drush 8.

## Example Playbook:
```
---
- name: Install Drush
  become: yes
  become_method: sudo
  hosts: 127.0.0.1
  connection: local

  vars:
    php_pkgs:
      - php
      (other php packages as desired)

  roles:
    - uclalib_role_php
    - uclalib_role_drush
```
