Role Name
=========
# Install Zabbix Agent with Ansible 
With this playbook, you can install Zabbix-agent on all versions of Debian/Ubuntu and versions 7 or 8 of RHEL/Centos machines.

Requirements
------------

- ansible version >= 2.10.4
- SSH access on machines
- sudo access on machines

Role Variables
--------------

1. Edit the playbook specific variables based on requierments
2. Specify target hosts in the form of [patterns](https://docs.ansible.com/ansible/latest/user_guide/intro_patterns.html) in the specific playbook

Dependencies
------------

- ansible
- ansible-playbook

Example Playbook
----------------


    # Replace {{ ROLE }} and {{ INVENTORY }} with the role and inventory name
    # Remove {{ TAGS }} and {{ SKIP_TAGS }} if not needed
```
ansible-playbook -i inventories/hosts --tags {{ TAGS }} --skip-tags {{ SKIP_TAGS }} playbooks/zabbix-agent/main.yml
```

License
-------

MIT

Author Information
------------------

* **Sadegh Khademi** - *SRE/Cloud Engineer* - Sadegh Khademi [website](https://sadeghkhademi.com) - Twitter [@niiiixd](https://twitter.com/niiiixd) - Email Address [Email](mailto:khademi.sadegh@gmail.com?subject=[GitHub]%20ansible%20zabbix%20agent)
