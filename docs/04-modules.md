##### Packages general
#####  https://docs.ansible.com/ansible/latest/modules/modules_by_category.html

###### Installing nginx and mysql with apt
###### https://docs.ansible.com/ansible/latest/modules/list_of_packaging_modules.html
```bash
cd source/apt
$ ansible-playbook loadbalancer.yml -i development
$ ansible-playbook database.yml -i development
```

###### Installing multiple packages
```bash
cd source/apt
$ ansible-playbook webserver.yml -i development
```

###### Using system modules (service)
###### https://docs.ansible.com/ansible/latest/modules/list_of_system_modules.html