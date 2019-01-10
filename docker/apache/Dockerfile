# Base Image of the Container.

FROM ubuntu:16.04

# Maintiner. 
MAINTAINER Amit Vashist

# APT _GET Update
RUN apt-get update -y

# Install Apache Packages 
RUN apt-get install apache2 -y

# Inject / Copy Index.html
COPY index.html /var/www/html/index.html

# When Container Start will the following commands
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND" ]

# Expose the Service
EXPOSE 80
