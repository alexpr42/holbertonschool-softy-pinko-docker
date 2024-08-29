# Use the latest official Nginx image as the base
FROM nginx:latest

# Copy the front-end files to the Nginx web directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the custom Nginx configuration file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
