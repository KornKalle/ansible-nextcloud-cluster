Ansible Nextcloud Cluster
=========

This role installs Nextcloud as a cluster setup on Debian >= Buster, Ubuntu >=18.04 and CentOS 8 with nginx and php7.4-fpm.

Requirements
------------

- Ansible >= 2.9
- kornkalle.ansible_nginx
- kornkalle.ansible_php74_fpm

Role Variables
--------------

TODO

Dependencies
------------

This role is developed for a system which used the role [kornkalle.ansible_nginx](https://github.com/KornKalle/ansible-nginx) for
installing nginx and the role [kornkalle.ansible_php74_fpm](https://github.com/KornKalle/ansible-php74-fpm) for installing php-fpm.

Future modifications could be agnostic about this for allowing custom nginx vHosts.  
Pull Requests are welcome.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: nextcloud-cluster
      roles:
        - { role: kornkalle.ansible_nginx }
        - { role: kornkalle.ansible_php74_fpm }
        - { role: kornkalle.ansible_nextcloud_cluster }

License
-------

MIT

Author Information
------------------

n.berg@backslashseven.de
