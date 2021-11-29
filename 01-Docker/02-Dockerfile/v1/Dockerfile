# Base Image 
FROM ubuntu:16.04

# Update the Apt Repo
RUN apt-get update 

# Install Apache Packages
RUN apt-get install apache2 -y 

# Bring up Apache. 
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
