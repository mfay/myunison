FROM alpine:latest

RUN apk update
RUN apk add vim unison supervisor

RUN mkdir - /etc/supervisor.d/
COPY unison.ini /etc/supervisor.d/.
RUN mkdir /host_sync
RUN mkdir /app_sync

CMD ["supervisord", "-n"]


