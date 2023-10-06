# Домашнее задание к занятию "`Система мониторинга Zabbix»`" - `Степанов Владислав`

### Задание 1

1.![Image alt](https://github.com/vladislst/hw-02/raw/main/img/zabbix.png)
2.
wget https://repo.zabbix.com/zabbix/6.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_6.0-4+ubuntu22.04_all.deb
dpkg -i zabbix-release_6.0-4+ubuntu22.04_all.deb
apt update
sudo -u postgres createuser --pwprompt zabbix
sudo -u postgres createdb -O zabbix zabbix
zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix
systemctl restart zabbix-server zabbix-agent apache2
systemctl enable zabbix-server zabbix-agent apache2

### Задание 2

1.![Image alt](https://github.com/vladislst/hw-02/raw/main/img/1.png)
2.![Image alt](https://github.com/vladislst/hw-02/raw/main/img/2.png)

