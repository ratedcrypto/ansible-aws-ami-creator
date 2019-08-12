# ansible-aws-ami-creator

## Features:
* Included ansible roles to create ec2 instance, refresh dynamic inventory, install-packages (java, php, composer, docker and docker-compose in this case), create ami and termiante ec2 instance
* Support for AWS environment variables in group_vars
* Support for role specific varialbes in defaults/main.yml

## Quick start

```bash
# Add ssh agent forwarding to ansible.cfg
nano /etc/ansible/ansible.cfg

# Add following in ansible.cfg
[ssh_connection]
ssh_args=-o ForwardAgent=yes

# Run the playbook
ansible-playbook -i hosts site.yml
```

## References
* https://github.com/geerlingguy/ansible-role-docker
* https://github.com/geerlingguy/ansible-role-java
* https://github.com/geerlingguy/ansible-role-php
* https://github.com/geerlingguy/ansible-role-composer