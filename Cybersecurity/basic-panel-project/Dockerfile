# Lightweight image of my classmate Antoine 
FROM alpine:latest

# Reduced the size of the image from 30,7 Mo to 28,43 Mo by including the --no-cache option
RUN apk add --no-cache apache2 php$phpverx-apache2

RUN rm -rf /var/www/localhost/htdocs

COPY . /var/www/localhost/htdocs

EXPOSE 80

CMD ["httpd", "-D", "FOREGROUND"]