FROM caddy:2.7.6-alpine

RUN apk add --no-cache \
bash \
bind-tools

COPY Caddyfile /etc/caddy/Caddyfile
COPY scripts /scripts
RUN chmod u+x /scripts/*

ENV VIKUNJA_SERVER_HOSTNAME=vikunja-server

CMD ["/scripts/start.sh"]
