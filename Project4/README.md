# Part 2
- Screenshot of host setup;
 - ![hostsetup](ceg3120-makaylac02/Project4/screenshots/host.PNG?raw=true "Host Setup") 
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
- Configs set: 
- Where site content files were located and why:
- How to restart the service after a config change: sudo systemctl start apache2
- Resources used:
  - https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-ubuntu-20-04



