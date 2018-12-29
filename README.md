# Ansible Playbooks pour HomeBox

## Installation d'ansible :

```bash
echo "deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main" | sudo tee -a /etc/apt/sources.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt-get update
sudo apt-get install -y ansible
```

## Installation et exécution du playbook sur le raspberry de sonde :

```bash
ansible-playbook playbooks/playbook-probe.yml
```
BME280 branché sur ?
DHT branché sur ?

## Installation et exécution du playbook sur le raspberry d'UI :
Note : Un Raspberry Pi peut acceuillir une sonde et l'UI simultanément

```bash
ansible-playbook playbooks/playbook-probe.yml
```
RF Branché sur ?

