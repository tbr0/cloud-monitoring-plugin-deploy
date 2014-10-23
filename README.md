An ansible playbook to install Cloud Monitoring plugins on the localhost.   This guide will not go into how to install ansible or git for your system.

Instructions:

```ansible-playbook -i hosts <playbook>```

###Available playbooks 
- mysql_slave.yml
- holland_mysqldump.yml
- port_check.yml (defaults to localhost:22)

###Examples
|Playbook | Arguments | Examples
| ---------- | ---------- | -------- |
| mysql_slave.yml | none | `ansible-playbook -i hosts mysql_slave.yml`
| holland_mysqldump.yml | none | `ansible-playbook -i hosts holland_mysqldump.yml`
| port_check.yml | host, port | `ansible-playbook -i hosts port_check.yml -e port=8080` \n `ansible-playbook -i hosts port_check.yml -e host=8.8.8.81

References:
- http://docs.rackspace.com/cm/api/v1.0/cm-devguide/content/install-configure.html#agent-config-file
- https://github.com/racker/rackspace-monitoring-agent-plugins-contrib
