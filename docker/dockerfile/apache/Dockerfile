# Base Image
FROM ubuntu:latest

# Owner
MAINTAINER Amit <amitvashist7@gmail.com>

# Update the Apt-Get Repo.
RUN apt-get update

# Install Apache Packages
RUN apt-get install apache2 -y 

# Inject the App. Code into Image. 
COPY index.html /var/www/html/index.html

# EXPOSE the Service
EXPOSE 80

# Bring Apache Service
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"] 
