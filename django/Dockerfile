FROM python:2.7

MAINTAINER "Nithesh Mittapally" <nithesh.chandra@gmail.com>

ENV APP_ROOT /usr/src/app
ENV UPLOADS_ROOT /var/local/app/uploads
ENV DJANGO_SETTINGS_MODULE web.settings.development
RUN mkdir -p "$APP_ROOT" "$UPLOADS_ROOT"
WORKDIR $APP_ROOT

EXPOSE 8000

CMD pip install -r requirements.txt && supervisord -c supervisord.conf
