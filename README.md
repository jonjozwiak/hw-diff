Role Name
=========

Hardware Drift Check 

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
See defailts/main.yml for variables

Dependencies
------------
None

Example Playbook
----------------

    - hosts: all
      vars:     
        hwinfo_path: "/tmp"
        delete_after_age: 4w
      # Do NOT gather facts prior to this playbook or it will break the diff check
      gather_facts: false
      roles:
         - jonjozwiak.hw-diff

License
-------

GPLv3

Author Information
------------------
Jon Jozwiak 
