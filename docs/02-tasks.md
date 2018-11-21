###### ping command
###### https://docs.ansible.com/ansible/latest/modules/ping_module.html
```bash
ansible -i development -m ping all
```
###### commands
###### https://docs.ansible.com/ansible/latest/modules/command_module.html
```bash
ansible -i development -m command -a "hostname" all
```