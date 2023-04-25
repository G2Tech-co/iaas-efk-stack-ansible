# G2 Fluentd Ansible IaC (Infrastructure as code)

[Ansible doc](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
[fluentd doc](https://docs.fluentd.org/container-deployment/docker-compose)

## Roles
- [x] Essentials
- [x] Swap
- [x] Docker
- [x] Elasticsearch
- [x] Fluentd
- [x] Kibana
- [x] Reboot

## Setup
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run
Add ssh config host name to `hosts`
```
ansible-playbook setup.yml
```

## Vault
```
echo $(htpasswd -nB user) | sed -e s/\\$/\\$\\$/g
```

## Defaults
```
Swap: 2G
```
