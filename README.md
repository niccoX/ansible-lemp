# Ansible LEMP installation

Will deploy a LEMP server with additional misc packages and copy over templated configuration files. 

### Installation

Install Ansible on your local host:

```sh
$ apt-add-repository ppa:ansible/ansible
$ apt-get update
$ apt-get install ansible
```

### Commands

Execute a run from the specific hosts in the inventory file:

```sh
$ ansible-playbook -i hosts playbook.yml
```

### Inventory File

Different ways to use credentials with the hosts inventory file

```sh
ansible_ssh_host
  The name of the host to connect to, if different from the alias you wish to give to it.
ansible_ssh_port
  The ssh port number, if not 22
ansible_ssh_user
  The default ssh user name to use.
ansible_ssh_pass
  The ssh password to use (this is insecure, we strongly recommend using --ask-pass or SSH keys)
ansible_ssh_private_key_file
  Private key file used by ssh.  Useful if using multiple keys and you don't want to use SSH agent.
```
