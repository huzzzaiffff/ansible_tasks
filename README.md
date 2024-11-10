# ansible_tasks

task-1:
create a variable file called secret.html which consists two below variables
pkg: httpd
srv: firewalld
this file should be encrypted and you need to create a playbook which print above variable.password of this file should be ansible and should store in pass.txt and playbook should take password directly from the file only

task-2:
create a playbook called packages.yaml that run in all managed node
install php and mariadb in webservers host group.
install Development Tools group of packages on dbservers host group.
update all packages on appservers host group.

task-3:
create a playbook called web.yaml run on dbservers host group with following (install httpd pkg first )
create a /webdev directory with the followings:
wheel is the group owner of the /webdev with permission u=rwx,g=rwx,o=r-x with sgid.
create a symbolic link between /var/www/html/webdev to /webdev.
create the file /webdev/index.html with asingle line of text that says "Development"
