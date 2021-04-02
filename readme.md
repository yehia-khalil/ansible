# Apache on Ubuntu 20.04

This playbook will install the Apache 2 web server and adding 2 virtual hosts on 2 ubuntu different machines, jusy type 
$ ansible-playbook -i hosts playbook.yml


## Settings

- `app_user`: a remote non-root user on the Ansible host that will own the application files.
- `http_host`: your domain name.
- `http_conf`: the name of the configuration file that will be created within Apache.
- `http_port`: HTTP port, default is 80.
- `disable_default`: whether or not to disable the default Apache website. When set to true, your new virtualhost should be used as default website. Default is true.

note :
 - you have to rewrite your machines configurations on hosts file 
 - yiu have to add your machines ip to the known list of the ssh just type : 
        - ssh <ip>
