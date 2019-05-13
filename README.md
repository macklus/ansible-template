# ansible base template

Ansible base template and structure

You can get more info about ansible on:
 * [Spanish](https://www.macklus.net/es/devops-es/ansible-es/conceptos-basicos-de-ansible/)
 * [English](https://www.macklus.net/en/devops-en/ansible-en/ansible-basics/)

## Install ansible on local PC

Install ansible on your computer, by running:
```bash
sudo add-apt-repository --yes ppa:ansible/ansible
sudo apt-get -y install ansible ansible-lint
sudo perl -pi -e 's/#host_key_checking = False/host_key_checking = False/ig' /etc/ansible/ansible.cfg
```

## Install ansible requirements

Install requirements or dependencies by running:
```bash
ansible-galaxy install **insert here your galaxy plugins**
```

## Your current playbooks

Reference here the playbooks you are defined, with their launch command, like:

```bash
ansible-playbook -i inventory/hosts examplePlaybook.yml
```

# Roles

## checks

### checks/define_hostname

Verify that system hostname is same that declared hostname (protection on license expired)