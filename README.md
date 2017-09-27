# DevopsProject
Code Challenge

Used Ansible for nginx installations

1. Created Ec2 instance in aws using S3.
2. Installed ansible on local node.
3. Using Nginx.yml downloaded the Nginx Package from svn repo. And installed the nginx.
4. It will also generate open ssl and create a directoty to save the keys.
5. default.conf.j2 template used for nginx conf. Which includes port redirection from 80 to 443.
6. Added test.html file in /usr/share/nginx/test.html. Nginx will host the file on port 443(HTTPS).
7. Nginx.yml also start the service once default.conf.j2 template deployed.
8. hosts file has client node to apply on.
