FROM almalinux:9

# Install nginx and curl
RUN dnf install -y nginx curl

# Remove default index.html
RUN rm -rf /usr/share/nginx/html/index.html

# Download index.html properly
RUN curl -o /usr/share/nginx/html/index.html https://raw.githubusercontent.com/daws-84s/notes/main/session-01.txt

# Ensure file permissions (optional)
RUN chmod +r /usr/share/nginx/html/index.html

# Start nginx in foreground
CMD ["nginx", "-g", "daemon off;"]
