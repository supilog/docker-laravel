FROM nginx:1.22

RUN mkdir /etc/nginx/sites-enabled
RUN mkdir -p /usr/local/nginx/vhosts/laravel.local.com/logs

COPY ./conf/nginx.conf /etc/nginx/nginx.conf
COPY ./conf/default.conf /etc/nginx/sites-enabled/default.conf

WORKDIR /usr/local/nginx/vhosts/laravel.local.com/htdocs
