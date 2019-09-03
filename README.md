# aws_https_to_nginx_ec2

To demostrate I have used nginx as a reverse proxy to access Kibana from the public IP address. 

To install nginx, run:

*sudo apt-get install nginx*

create a basic authentication file with the OpenSSL command:

*echo "admin:$(openssl passwd -apr1 YourStrongPassword)" | sudo tee -a /etc/nginx/htpasswd.kibana*

Installing ELK ELB Instance https://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-create-https-ssl-load-balancer.html

configuring Nginx /etc/nginx/site-available/kibana.conf
