FROM nginx

COPY . /usr/share/nginx/html

# run nginx with "foreground mode" to not exit Docker
ENTRYPOINT ["nginx", "-g", "daemon off;"]