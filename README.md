# ansible_samples
Ansible playbooks for some of my personal test environments. Setup dev environment as follows:

1. install Virtualbox (download installer from web)
1. install Vagrant (brew install vagrant)
1. install Ansible (brew install ansible)
1. copy ssh key to remote servers (ssh-copy-id "servername">)
1. create a file named root_pw.txt in the current folder with become password in it
1. run a playbook (ansible-playbook site.yml --check)
   will be prompted to enter sudo password for remote system
1. run test through vagrant (TBD)

# Links

- https://www.vagrantup.com/docs/provisioning/ansible

# Todo

- set up passwordless sudo on servers
- document ssh key handling
- figure out dynamic inventory with vagrant
- see if I can set a default playbook file (ie: site.yml)

# Samples

- ansible all -m ping
- ansible-playbook site.yml
- ansible-playbook site.yml --limit minecraft
- ansible-playbook site.yml --limit homeserver1
- ansible-playbook site.yml --check
