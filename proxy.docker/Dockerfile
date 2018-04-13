FROM debian-base

COPY sockd.conf /etc/

CMD useradd --shell /usr/sbin/nologin ${PROXY_USERNAME} \
    && echo "${PROXY_USERNAME}:${PROXY_PASSWORD}" | chpasswd \
    && sockd
