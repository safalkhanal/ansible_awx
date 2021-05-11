ansible_role_awx
=========

This role installs Ansible AWX.
Note: This role installs Ansible AWX version 17.1.0 or less.

Requirements
------------
Before using this role, docker must be installed. Following role can be used to install docker before installing AWX.

respiro.ansible_role_docker

Role Variables
--------------
postgres_data_dir : location of where postgres data will be kept.

awx_version : The version of AWX to be installed.

awx_repo_dir : Directory path to install AWX.

Dependencies
------------
VM is needed to install. Tested with following OS:

Ubuntu 18.04 (Bionic)

Example Playbook
----------------

    - hosts: servers
      become: yes
      roles:
         - respiro.ansible_role_docker
         - respiro.ansible_role_awx

License
-------

MIT / BSD
