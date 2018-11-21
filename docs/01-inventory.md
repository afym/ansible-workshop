###### startup the project

```bash
docker-compose exec ansible bash
```

###### list your hosts for your inventory

```bash
ansible --list-hosts all
```

###### The global hosts file will be located in
```bash
/etc/ansible/hosts
```

###### list your hosts for your inventory

```bash
cd /home/project
ansible -i development --list-hosts all
```

###### using the local configuration file for your project (ansible.cfg in the project)

```bash
cd /home/project
ansible --list-hosts all
```

###### Pattern options for list hosts
###### https://docs.ansible.com/ansible/latest/user_guide/intro_patterns.html
```bash
cd /home/project
ansible --list-hosts "*"
ansible --list-hosts loadbalancer
ansible --list-hosts webservers
ansible --list-hosts db01
ansible --list-hosts app0*
ansible --list-hosts webservers[0]
ansible --list-hosts webservers:database
ansible --list-hosts \!webservers
```