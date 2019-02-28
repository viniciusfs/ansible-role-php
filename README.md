# Ansible role: PHP 7

[![Build Status](https://travis-ci.org/viniciusfs/ansible-role-php.svg?branch=master)](https://travis-ci.org/viniciusfs/ansible-role-php)

Installs PHP 7 from remi repositories on RHEL/CentOS systems.


## Role Variables

* `php_packages`:
    - Description: List of PHP packages to install
    - Default: `[ 'php72', 'php72-php', 'php72-php-cli', 'php72-php-common' ]`


## Example Playbook

    - hosts: workstations
      roles:
        - name: viniciusfs.php
          php_packages:
            - php72
            - php72-php
            - php72-php-cli
            - php72-php-common
            - php72-php-gd
            - php72-php-mstring
            - php72-php-mysqlnd
            - php72-php-ldap


## License

MIT


## Author Information

* Vinícius Figueiredo <viniciusfs@gmail.com>
