# Ansible playbook to setup a shell box
A Vagrantfile is included to test or modify the playbook further

## Setup shell box
* We need to install ansible first
* The user needs to be able to run sudo without password
```
sudo apt update && sudo apt install -y ansible
ansible-playbook -i inventory playbook.yml
```

## Test the playbook using vagrant
If doing this at work where a proxy is being used, you need to use an image that has a proxy cert imbedded in it and set the NODE_EXTRA_CA_CERTS environment for pyright installation
```
vagrant up
```

## TODO
* install docker-ce
* install linuxbrew
* install fd
* install ripgrep
* install bat
* install jq
* install jless
* install klog
