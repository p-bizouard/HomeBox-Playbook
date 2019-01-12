# Ansible Playbooks pour HomeBox

## Installation d'ansible :

```bash
sudo apt-get install -y dirmngr git
echo "deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main" | sudo tee -a /etc/apt/sources.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt-get update
sudo apt-get install -y ansible
```

## Installation et exécution du playbook sur le raspberry de sonde :

```bash
git clone https://github.com/p-bizouard/homebox-playbook-ansible.git
cd homebox-playbook-ansible
ansible-playbook playbooks/playbook-probe.yml
```

## Installation et exécution du playbook sur le raspberry d'UI :
Note : Un Raspberry Pi peut acceuillir une sonde et l'UI simultanément

```bash
git clone https://github.com/p-bizouard/homebox-playbook-ansible.git
cd homebox-playbook-ansible
ansible-playbook playbooks/playbook-ui.yml
```

## Todo
- [X] Passer sur pm2
