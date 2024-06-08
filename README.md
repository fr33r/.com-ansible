# .com-ansible

Various Ansible artifacts (playbooks, etc.) used to maintain fr33r.com.

## Initial Setup Instructions

### Control Node

#### MacOS

```bash
> brew install ansible
```

#### Linux

```bash
> sudo apt-get install ansible
```

### Example Commands

```bash
ansible-playbook -i inventory/hosts playbooks/install-nfs-client.yml -e "target_hosts=picluster" -u <USER> --become --ask-become-pass --ask-pass
```
