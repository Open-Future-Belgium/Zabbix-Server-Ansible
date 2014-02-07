Zabbix-Server-Ansible
=====================

Zabbix Server module for ansible

How To:
-------
1. Edit the zabbix-server.yml file and add replace host
2. Edit files in directory defaults and change variables to your needs
3. Install with tags if u want to exclude apache, postgres or zabbix 
4. ansible-playbook zabbix-server.yml --tags "postgres,http,zabbix"
5. Else just run ansible-playbook zabbix-server.yml

