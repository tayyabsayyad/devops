
# 1. Installing, Configuring, and Running Ansible

### To install Ansible on ubuntu distribution

      sudo apt-get update
      sudo apt-get install software-properties-common
      sudo apt-add-repository ppa:ansible/ansible
      sudo apt-get update
      sudo apt-get install ansible

### Install Via Python pip
      sudo pip install ansible
      sudo pip install ansible


### Verify ansible is installed properly and functioning
      ansible --help
      ansible --version

## Features of Ansible
  - Open source   https://github.com/ansible/ansible
  - Module-based - developed for integration with numerous other open and closed source software solutions.
  - Agentless - This means there are no daemons that need to be installed on remote machines, no firewall ports that need to be opened (besides traditional SSH)
  - Pluggable - Can be plugged with the internal softwares
  - Local automation execution using Ansible

## Local machine configuration management

    $ansible all -i "localhost," -c local -m shell -a 'echo hello DevOps World'

 Command simply tells Ansible to target all systems in the ad hoc inventory implementation (which in our simple use case is only localhost), then execute the command echo "hello DevOps world" against this system.

 ## Playbook Example Local

 Open the File hellodevopsworld.yml

    $ansible-playbook -i 'localhost,' -c local hellodevopsworld.yml

 ## Remote automation execution using Ansible
      ansible-playbook -i "192.168.1.148," -c local hellodevopsworld.yml
