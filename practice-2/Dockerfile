FROM alpine:3.2

RUN apk add --update nginx && rm -rf /var/cache/apk/*

#COPY nginx.conf /etc/nginx/nginx.conf
COPY nginx.non-root.conf /etc/nginx/nginx.conf
COPY index.html /var/www/html/index.html
#COPY index.html /usr/share/nginx/html/index.html


USER  nobody
CMD ["nginx", "-g", " daemon off;"]
