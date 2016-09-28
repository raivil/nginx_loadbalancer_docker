FROM haproxy:latest

RUN useradd -r haproxy
RUN mkdir -p /etc/haproxy
RUN mkdir -p /run/haproxy
RUN mkdir -p /var/lib/haproxy
RUN touch /var/lib/haproxy/stats
COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
