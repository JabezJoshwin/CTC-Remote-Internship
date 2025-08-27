# Use the official Nginx image from Docker Hub
FROM nginx:alpine

# Remove the default nginx static site
RUN rm -rf /usr/share/nginx/html/*

# Copy your "final" folder contents to the container's web root
COPY . /usr/share/nginx/html/

# Expose the default HTTP port
EXPOSE 80

# Start Nginx in the foreground (as the container's main process)
CMD ["nginx", "-g", "daemon off;"]
