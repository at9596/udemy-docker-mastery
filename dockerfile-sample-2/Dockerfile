# this shows how we can extend/change an existing official image from Docker Hub

FROM nginx:latest


WORKDIR /usr/share/nginx/html
# change working directory to root of nginx webhost
# using WORKDIR is preferred to using 'RUN cd /some/path'

COPY index.html index.html


# How do i run:
    # docker container run -p 80:81 nginx-with-html
    # docker container run -p 81:80 nginx-with-html
    # Heads up to your browser and go to: http://localhost:81/
