# ansible-role-opensips
![License](https://img.shields.io/github/license/mach1el/ansible-role-archlinux?color=purple&style=plastic)
Auto building,config opensips sip proxy

## Role pathes

    ├── defaults
    │   └── main.yml
    ├── handlers
    │   └── main.yml
    ├── tasks
    │   ├── control_panel_installation.yml
    │   ├── do_log.yml
    │   ├── main.yml
    │   └── setup_debian.yml
    └── templates
        ├── config
        │   ├── apache2.conf.j2
        │   ├── cdr_viewer.php
        │   ├── db.inc.php.j2
        │   ├── local.inc.php.j2
        │   ├── opensips.cfg.j2
        │   └── opensipsctlrc.j2
        └── scripts
            └── create_column.sql

## Role Playbook
	---
	- name: Building archlinux for local server
	  hosts: local
	  roles:
	  	- '/ansible-role-opensips'
