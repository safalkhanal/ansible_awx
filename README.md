deploy_awx
=========

This role installs Ansible AWX

Requirements
------------
This role needs to be used with following role:
respiro.install_docker

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
         - role: respiro.deploy_awx 

License
-------

MIT / BSD
