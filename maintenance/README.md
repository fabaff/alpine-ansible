# Maintenance

The playbooks in this directory performs maintenance task, like updating
packages, upgrading systems, cleaning systems, or what else is useful. No
task is depending on other files. 

## update.yml 
All installed packages are updated and the system will reboot after the package 
update task is over. In the current configuration it doesn't make sense to run
this playbook every hour because of the system reboot.
For additional details please refer to this [section](http://wiki.alpinelinux.org/wiki/Alpine_Linux_package_management#Upgrade_a_Running_System) in the Alpine Linux wiki.

## clean-cache.yml
The cache directory is storing all versions of a package. Over time the cache is filled
because newer packages will replace older ones. This playbook is cleaning the cache.

For additional details please refer to this [section](http://wiki.alpinelinux.org/wiki/Alpine_Linux_package_management#Delete_old_packages) in the Alpine Linux wiki.

## lighttpd.yml
The *lighttpd.yml* playbook installs the [lighttpd](http://www.lighttpd.net/) 
web server with [FastCGI](www.fastcgi.com/) support and PHP.

## linfo.yml
[Linfo](http://linfo.sourceforge.net/) is a simple PHP application that
displays information about the host it's running on. A running lighttpd server
is needed. This means, run the **lighttpd.yml** first.
