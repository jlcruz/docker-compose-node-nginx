FROM nginx

MAINTAINER crux



# Copy a configuration file from the current directory
ADD app.conf /etc/nginx/conf.d/

RUN rm -v /etc/nginx/conf.d/default.conf

# Append "daemon off;" to the beginning of the configuration
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

# Create directory for storing App or UI code and copy sample index.html
RUN ["mkdir", "/usr/share/nginx/html/app"]
ADD index.html /usr/share/nginx/html/app/

# Expose ports
EXPOSE 80

# Set the default command to execute
# when creating a new container
CMD service nginx start
