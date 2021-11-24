# Ansible Collection

### How to use:
1. Edit the playbook specific variables based on requierments
2. Specify target hosts in the form of [patterns](https://docs.ansible.com/ansible/latest/user_guide/intro_patterns.html) in the specific playbook
3. Run the playbook
-  Run playbooks

        # Replace {{ ROLE }} and {{ INVENTORY }} with the role and inventory name
        # Remove {{ TAGS }} and {{ SKIP_TAGS }} if not needed
        ansible-playbook -i inventories/{{ INVENTORY }} --tags {{ TAGS }} --skip-tags {{ SKIP_TAGS }} playbooks/{{ ROLE }}/main.yml --ask-become-password
