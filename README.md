An ansible playbook to install Cloud Monitoring plugins on the localhost.   This guide will not go into how to install ansible or git for your system.

Instructions:

```ansible-playbook -i hosts <playbook>```

###Available playbooks 
- mysql_slave.yml
- holland_mysqldump.yml

References:
- http://docs.rackspace.com/cm/api/v1.0/cm-devguide/content/install-configure.html#agent-config-file
- https://github.com/racker/rackspace-monitoring-agent-plugins-contrib
