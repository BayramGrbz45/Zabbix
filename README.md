# Denomas Monitoring  6.0

## Preliminary

- 2 Adet Ubuntu 20.04 (Ansible - Zabbix Server)

- Ansible server kurulumu.

    - /etc/hosts **monitoring ip ve url**
    - sudo apt update && sudo apt upgrade -y
    - sudo apt install build-essential python3-virtualenv virtualenv python3-dev libffi-dev libssl-dev libsasl2-dev libldap2-dev python3-pip sshpass -y
    - virtualenv /opt/venv/zbx_ansible/ --python=python3
    - cd /opt/venv/
    - source zbx_ansible/bin/activate
    - pip3 install --upgrade setuptools wheel pip
    - pip3 install ansible
    - pip3 install netaddr zabbix-api grafana-api pywinrm[credssp]
    - git clone https://github.com/BayramGrbz45/Zabbix.git
    - cd Zabbix
    - ansible-galaxy install -r roles/requirements.yaml

### Services 

* Checked services are completed

- [x] Nginx
- [x] PHP
- [x] Postgresql
- [x] Zabbix Server
- [x] Zabbix Web
- [ ] Zabbix Javagateway
- [x] ODBC Install
- [x] Zabbix Agent2 PSK (Linux - Windows) 
- [x] Zabbix & Monitoring  Find-Replace
- [x] Zabbix Host Group Create and Choose (All  Hosts, Windows Servers ... )
- [x] Zabbix Host Create and Update 
- [x] Zabbix User Create and Update
- [x] Zabbix User Group Create and Choose (Admin, Monitoring ...)
- [x] Zabbix Mediatype (Mail)

## Future Work
- Zabbix turkish language
- Zabbix Proxy
- Elasticsearch
- zabbix discovery_rule
- zabbix globalmacro
- zabbix maintenance
- zabbix maps
- zabbix service
- zabbix valuemap
- Zabbix Javagateway
- Zabbix SNMP Host Add (v1 -  v2 - v3)
- Zabbix Screen (Linux - Windows)
