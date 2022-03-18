# Part 2 
## To switch between the 2 instances, I added my private key to the proxy server and was then able to use the key to ssh into webserv1 and webserv2
### Commands for ssh: 
#### webserv1: ssh -i ceg2350.pem ubuntu@10.0.1.10
#### webserv2: ssh -i ceg2350.pem ubuntu@10.0.1.11
