Ansible Playbook: postgresql-host
=================================

Configure PostgreSQL database server

Supported OS:
-------------
* RedHat
* CentOS
* OracleLinux

Requirements
------------

This playbook requires the postgresql-host role.

`$ ansible-galaxy install -r roles/requirements.yml`

Examples
--------

    $ ansible-playbook playbook.yml --list-tasks
    $ ansible-playbook playbook.yml --list-tags

Complete PostgreSQL database server configuration

    $ ansible-playbook playbook.yml

Configure common services (ntp/motd)

    $ ansible-playbook playbook.yml --tags=postgresql_host_services

Disable transparent hugepages

    $ ansible-playbook playbook.yml --tags=postgresql_host_transparent_hugepages

Disable SElinux

    $ ansible-playbook playbook.yml --tags=postgresql_host_selinux

Configure firewall

    $ ansible-playbook playbook.yml --tags=postgresql_host_firewall

Configure tuned profile

    $ ansible-playbook playbook.yml --tags=postgresql_host_tuned

Configure postgres OS user

    $ ansible-playbook playbook.yml --tags=postgresql_host_postgres_group,postgresql_host_postgres_user
	
Configure DBA accounts

    $ ansible-playbook playbook.yml --tags=postgresql_host_dba_users

Configure postgres .bash_profile

    $ ansible-playbook playbook.yml --tags=postgresql_host_postgres_userprofile

Configure sudo entries

    $ ansible-playbook playbook.yml --tags=postgresql_host_sudoers

Configure filesystems

    $ ansible-playbook playbook.yml --tags=postgresql_host_filesystems

Configure NFS shares

    $ ansible-playbook playbook.yml --tags=postgresql_host_nfs

Configure dbpostgres service

    $ ansible-playbook playbook.yml --tags=postgresql_host_postgres_service

Copy standard scripts and files

    $ ansible-playbook playbook.yml --tags=postgresql_host_copy_files

Execute host customization

    $ ansible-playbook playbook.yml --tags=postgresql_host_customization

	
License
-------

GPLv3 - GNU General Public License v3.0

Author Information
------------------

This playbook was created in 2018 by [Krzysztof Lewandowski](mailto:Krzysztof.Lewandowski@fastmail.fm).


