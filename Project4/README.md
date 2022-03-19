# Part 2
### Setup
- Screenshot of host setup;
- ![hostsetup](screenshots/host.PNG?raw=true "Host Setup") 
- To switch between the 2 instances, I added my private key to the proxy server and was then able to use the key to ssh into webserv1 and webserv2
 - Commands for ssh: 
   - webserv1: ssh -i ceg2350.pem ubuntu@10.0.1.10
   - webserv2: ssh -i ceg2350.pem ubuntu@10.0.1.11

### HAProxy
- File modified: sudo nano /etc/haproxy/haproxy.cfg
- Configs set: 
- Restart command: sudo systemctl restart haproxy
- Resources:
   - https://www.haproxy.com/blog/the-four-essential-sections-of-an-haproxy-configuration/
   - https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/load_balancer_administration/install_haproxy_example1
   - https://upcloud.com/community/tutorials/haproxy-load-balancer-ubuntu/#:~:text=Setting%20up%20HAProxy%20for%20load,cfg%20with%20the%20defining%20settings.

### Webserver 1 and 2 Configs
- Files modified: 
  - Had to adjust firewalls: sudo ufw allow 'Apache'
- Configs set: 
  - Config block:
    - This is used from the website I linked as a resource:
    - <VirtualHost *:80>
    ServerAdmin carr.137@wright.edu
    ServerName webserver1 
    ServerAlias www.webserver1
    DocumentRoot /var/www/webserver1
    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
   </VirtualHost>
   - Repeated for server2
- Where site content files were located and why:
  - We store the content of the files on a virtural host so we can host more than one domain. The domain will hold our information.  
  - Command to edit: sudo nano /var/www/your_domain/index.html
- How to restart the service after a config change: sudo systemctl start apache2
- Resources used:
  - https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-ubuntu-20-04



