# Ansible LAMP installation

Will deploy a LAMP server with additional misc packages and copy over templated configuration files. 

### Installation

Install Ansible on your local host:

```sh
$ apt-add-repository ppa:ansible/ansible
$ apt-get update
$ apt-get install ansible
```

### Commands:

Execute a run from the specific hosts in the inventory file:

```sh
$ ansible-playbook -i hosts playbook.yml
```
