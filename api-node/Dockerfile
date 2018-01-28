############################################################
# Dockerfile to build Nginx Installed Containers
# Based on Ubuntu
############################################################

# Set the base image to Ubuntu
FROM node:alpine

# File Author / Maintainer
MAINTAINER crux



# Create directory for storing NodeJS or API code and copy sample index.js
RUN ["mkdir", "/home/nodejstest/"]
ADD index.js /home/nodejstest

# Expose ports
EXPOSE 9090

# Start NodeJS with sample program
CMD ["node", "/home/nodejstest/index.js"]

