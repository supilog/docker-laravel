FROM mysql/mysql-server:5.7.38

COPY ./conf/my.cnf /etc/my.cnf
RUN chmod 644 /etc/my.cnf

ENV MYSQL_ROOT_PASSWORD=63a9f0ea7bb98050796b649e85481845
ENV MYSQL_USER=laravel
ENV MYSQL_PASSWORD=dbc8958e9b2aaadea2eb8b1b3046d949
ENV MYSQL_DATABASE=laravel
ENV TZ=Asia/Tokyo


WORKDIR /usr/local/nginx/vhosts/laravel.local.com/htdocs
