# ansible-role.application_phpmyadmin

Install
========
```
git submodule add git@github.com:Waldz/ansible-role.application_phpmyadmin.git roles/application_phpmyadmin
```

Example
========
```
- name: Deploy basic tools to all servers
  hosts: all
  sudo: true
  roles:
    #- role: nginx
    - role: application_phpmyadmin
```

Variables
========
group_vars/all.yml
```
---
phpmyadmin_path_public: /var/www/default/pma

phpmyadmin_db_name: phpmyadmin
phpmyadmin_db_user: phpmyadmin
phpmyadmin_db_pass: SuPerPassWorD
```
