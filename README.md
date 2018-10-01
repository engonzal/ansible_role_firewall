ansible_role_users
=========

Ansible role to provision firewall allowed ports.

Role Variables
--------------

Create a list of ports to use in this format (note do not use "quotes"):
```yaml
firewall_allow:
  - 3000
firewall_allow_tcp:
  - 22
```

Example Playbook
----------------

    - hosts: servers
      vars:
        firewall_allow:
          - 3000
      roles:
        - { role: engonzal.ansible_role_firewall, tags: [ 'firewall'] }

License
-------

BSD

Author Information
------------------

Noe Gonzalez - http://engonzal.com
