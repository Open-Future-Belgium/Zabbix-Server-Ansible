Zabbix Server
=============

This playbook will install the Zabbix Server with postgresql and apache if needed.

1. Edit the zabbix-server.yml file and add replace host
2. Edit files in directory defaults and change variables to your needs
3. Install with tags if u want to exclude apache, postgres or zabbix
4. ansible-playbook zabbix-server.yml --tags "postgres,http,zabbix"
5. Else just run ansible-playbook zabbix-server.yml

Requirements
------------

Everything will be installed automatic but at the moment the installation script only works on Redhat 6.x or Centos 6.x

Role Variables
--------------

All variables can be altered in the defaults directory. There are files for postgresql, zabbix and apache

Dependencies
------------

no other roles are used

Todo
----
1. add config for debian
2. add selinux
3. add iptables

License
-------

GPL V2

Author Information
------------------

Patrik Uytterhoeven
patrik( at )open-future.be
www.open-future.be

