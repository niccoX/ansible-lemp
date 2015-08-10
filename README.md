# Ansible LAMP installation

Will install a LAMP server with additional misc packages and copy over configuration files.

### Installation

Install Ansible:

```sh
$ apt-add-repository ppa:ansible/ansible
$ apt-get update
$ apt-get install ansible
```

#### Commands:

Execute a run from the specified hosts of the inventory file:

```sh
$ ansible-playbook -i hosts playbook.yml
```
