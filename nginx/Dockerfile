# Fixed "latests" to "latest"
FROM nginx:latest  

# Copy the Nginx configuration file
# Fixed "nginix.conf" to "nginx.conf"
COPY nginx.conf /etc/nginx/nginx.conf  

# Removed COPY ./html /usr/share/nginx/htmll

# Expose port 80 (use numeric values)
# Changed from "eighty" to the actual port number
EXPOSE 80  

# Start Nginx in the foreground
# Fixed "daemon of" to "daemon off"
CMD ["nginx", "-g", "daemon off;"]  
