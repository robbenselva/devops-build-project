# Stage 1: Use nginx to seerve the build files
FROM nginx:alpine

# Remove default ngiinx static content
RUN rm -rf /usr/share/nginx/html/*

# Copy your build outtput to Nginx document root
COPY /build/ /usr/share/nginx/html/

# Expose port 80
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]





