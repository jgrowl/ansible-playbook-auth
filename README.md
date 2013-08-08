ansible-playbook-auth
=====================

Ansible playbook to deploy/manage an authentication/authorization server

# Instructions

[Install the dpkg_reconfigure ansible plugin](https://github.com/ginsys/ansible-plugins/blob/devel/library/dpkg_reconfigure)

`cp -r .private.template .private`

`vi .private/vars/private.yml`

Adjust variables to your environment, and run!

# Notes

This script can take a long time to run because it has to create the krb realm.

# Disclaimer 

I can not guarantee everything here is 100% safe. Please use at your own risk.

# Credit

[Based on Dan Bishop's awesome Ultimate Server Guide!](http://www.danbishop.org/2012/06/02/ubuntu-12-04-ultimate-server-guide/)

