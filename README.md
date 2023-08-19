# free_SSL_certificate
To install a free SSL certificate on an Ubuntu EC2 instance running Apache2, you can use Let's Encrypt, which provides free SSL certificates. Here are the steps to install and configure Let's Encrypt on your EC2 instance with Apache2


Update your Ubuntu packages:
Before installing Let's Encrypt, update your system's package list to ensure you have the latest information about available packages.

#sudo apt update

 Install Certbot (Let's Encrypt client):
Certbot is a tool that simplifies the process of obtaining and renewing SSL certificates from Let's Encrypt. Install it using apt:

#sudo apt install certbot python3-certbot-apache

Obtain and Install the SSL Certificate:
Use Certbot to obtain and install your SSL certificate. Replace example.com with your domain name:

#sudo certbot --apache -d example.com -d www.example.com


#sudo apache2ctl configtest
#sudo systemctl reload apache2
