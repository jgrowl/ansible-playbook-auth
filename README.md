ansible-playbook-auth
=====================

Ansible playbook to deploy/manage an authentication/authorization ubuntu 12.04 server. Installs kerberos and ldap along with a basic ldap db.

# Instructions

[Install the dpkg_reconfigure ansible plugin](https://github.com/ginsys/ansible-plugins/blob/devel/library/dpkg_reconfigure)

`cp -r .private.template .private`

`vi .private/vars/private.yml`

Adjust variables to your environment, and run!

# Notes

This script can take a long time to run because it has to create the krb realm.

# Disclaimer 

I can not guarantee everything here is 100% secure. Please use at your own risk. Please let me know if you see an obvious issues.
The main thing is the script runs ldif commands passing the password on the command line. This is bad, I know but these commands
should only be run once when the box is getting set up. Still should be fixed though!


# Credit

[Based on Dan Bishop's awesome Ultimate Server Guide!](http://www.danbishop.org/2012/06/02/ubuntu-12-04-ultimate-server-guide/)

