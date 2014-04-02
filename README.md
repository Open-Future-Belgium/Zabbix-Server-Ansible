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

At this moment the script only works on Redhat 6.x or Centos 6.x
The zabbix-server script will install the Zabbix Server package from the zabbix repository with a PostgreSQL database and a Apache webserver.


Role Variables
--------------
All variables can be altered in the defaults directory.

httpd.yml
main.yml
postgresql.yml
zabbix.yml

Dependencies
------------

no other roles are used

Todo
----
1. add config for debian

License
-------

GPL V2

Author Information
------------------

* Patrik Uytterhoeven
* patrik( at )open-future.be
* [www.open-future.be](http://www.open-future.be)

