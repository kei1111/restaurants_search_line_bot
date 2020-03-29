FROM nginx:1.15.6-alpine
ENV APP_ROOT /usr/src/lineBot

RUN mkdir $APP_ROOT

COPY ./public $APP_ROOT/public
COPY ./docker/nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./docker/nginx/conf.d/lineBot.conf /etc/nginx/conf.d/lineBot.conf

EXPOSE 80
