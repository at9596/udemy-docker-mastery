# Use a modern, supported version of Debian or Nginx
FROM nginx:1.25-alpine

# Alpine already has Nginx set up, but if you want to 
# practice the log linking you had:
RUN ln -sf /dev/stdout /var/log/nginx/access.log \
    && ln -sf /dev/stderr /var/log/nginx/error.log

EXPOSE 80 443 8080

CMD ["nginx", "-g", "daemon off;"]
 