ELK
=========

Install elk stack 

Requirements
------------

Supported only Ubuntu OS

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

    - name: Install ELK
      hosts: elk_hosts
      gather_facts: no
      roles:
        - role: elk
          add_elasticsearch: yes
          add_kibana: yes
          add_logstash: yes
          kibana_dns_name: kibana.foo.org
          elasticsearch_cluster_name: dev-01


License
-------

BSD

