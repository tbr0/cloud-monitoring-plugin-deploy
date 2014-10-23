An ansible playbook to install Cloud Monitoring plugins on the localhost.   This guide will not go into how to install ansible or git for your system.

Instructions:

```ansible-playbook -i hosts <playbook>```

###Available playbooks 
- mysql_slave.yml
- holland_mysqldump.yml
- port_check.yml (defaults to localhost:22)

###Examples
|Playbook | Arguments (defaults) | Examples
| ---------- | ---------- | -------- |
| mysql_slave | | default
| holland_mysqldump | | default
| port_check | host=localhost <br> port=22 | port_check.yml -e host=1.2.3.4 <br> port_check.yml -e port=8080 <br> port_check.yml -e '{"host":"8.8.8.8","port":"53"}'

References:
- http://docs.rackspace.com/cm/api/v1.0/cm-devguide/content/install-configure.html#agent-config-file
- https://github.com/racker/rackspace-monitoring-agent-plugins-contrib
