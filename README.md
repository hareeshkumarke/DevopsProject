# DevopsProject

Used Ansible for nginx installations

step by step execution:

1. Created Ec2 instance in aws using S3.
2. Installs ansible on local node.
3. Using Nginx.yml downloaded the Nginx Package from svn repo and installed it.
4. It will also generate open ssl and creates a directoty to save the keys.
5. default.conf.j2 template used for nginx conf. Which includes port redirection from 80 to 443.
6. Added test.html file in /usr/share/nginx/test.html. Nginx will host the file on port 443(HTTPS).
7. nginx.yml will start the service once default.conf.j2 template is deployed.
8. hosts file explains the creation of instance and has client node to apply on.
