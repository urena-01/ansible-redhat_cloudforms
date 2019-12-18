cfme_health_check
=========

Perform a CFME Health Check

Requirements
------------

No Requirements

Role Variables
--------------

+ cfme_healthcheck_retries - how many times to try the CF /ping enpoint before marking node as failed
+ cfme_port_ready_timeout_seconds - how long to wait for port 443 to be ready

Dependencies
------------

No Dependencies

Example Playbook
----------------

```

---
- name: CFME | Health Check
  hosts: cfme_appliances
  gather_facts: True
  tasks:
    - name: CFME | Health Check | Include Tasks
      import_role:
        name: install_custom_facts
```

License
-------

Apache 2.0

Author Information
------------------

Developed by Red Hat Consulting. Community Supported. Please Open a GitHub Issue if you have any questions or encounter any issues.