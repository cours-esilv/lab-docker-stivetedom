# Use a lightweight web server as the base image
FROM nginx:alpine

# Set the working directory
WORKDIR /usr/share/nginx/html

# Copy the contents of the front directory into the container
COPY . .

# Set the entrypoint to execute any CMD as arguments to 'nginx'
ENTRYPOINT ["nginx", "-g", "daemon off;"]
