FROM ritukamboj27/nginx:latest
RUN apt-get update && apt-get install gettext-base
ENV PROXY_PROTOCOL=http PROXY_UPSTREAM=example.com
COPY proxy.conf /etc/nginx/sites-available/default.template
COPY stat.sh /
CMD ["/stat.sh"]

