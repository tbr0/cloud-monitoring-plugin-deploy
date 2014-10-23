An ansible playbook to install Cloud Monitoring plugins on the localhost.   This guide will not go into how to install ansible or git for your system.

Default command:

```ansible-playbook -i hosts <playbook>```

###Available playbooks 
- mysql_slave.yml
- holland_mysqldump.yml
- port_check.yml

###Examples
| Name | Arguments (defaults) | Examples
| ---------- | ---------- | -------- |
| mysql_slave | | mysql_slave.yml
| holland_mysqldump | | holland_mysqldump.yml
| port_check | host=localhost <br> port=**required** | port_check.yml -e port=8080 <br> port_check.yml -e '{"host":"rackspace.com","port":"80"}'

References:
- [Rackspace Cloud Monitorin API - Agent Config File](http://docs.rackspace.com/cm/api/v1.0/cm-devguide/content/install-configure.html#agent-config-file)
- [Github for Cloud Monitoring Agent Plugins](https://github.com/racker/rackspace-monitoring-agent-plugins-contrib)
