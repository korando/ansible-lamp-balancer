# Ansible LAMP-Balancer.

This is a simple recipe that sets up an Ubuntu virtual machine including common daemons and tools required for PHP web development.

All the provisioning is done with `Ansible`.

## LAMP environnement

This project is designed to install all needed for web server on a LAMP architecture.It will install the following on an Ubuntu 14.04 linux VM:

- Apache 2.4.x
- PHP 5.5.x
- MySQL 5.5.x
- Composer
- Git
- Xdebugs
- SSL
- Mongoclient
- Phalcon
- Vsftpd

and Load balancer (HAproxy)

Example command:

```ansible-playbook -i hosts apache.yml --tag=apache  -u 'root-user' --ask-sudo-pass```
