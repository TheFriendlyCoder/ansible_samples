# ansible_samples
Ansible playbooks for some of my personal test environments. Setup dev environment as follows:

1. install Virtualbox (download installer from web)
1. install Vagrant (brew install vagrant)
1. install Ansible (brew install ansible)
1. copy ssh key to remote servers (ssh-copy-id "servername">)
1. run a playbook (ansible-playbook site.yml --check -K)
   will be prompted to enter sudo password for remote system
1. run test through vagrant (TBD)

# Links

- https://www.vagrantup.com/docs/provisioning/ansible

# Todo

- set up passwordless sudo on servers
- document ssh key handling
- figure out dynamic inventory with vagrant