FROM nginx:1.15.3-alpine

COPY ./fastcgi_params /etc/nginx/fastcgi_params
COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./nginx-entrypoint.sh /nginx-entrypoint.sh

RUN chmod +x /nginx-entrypoint.sh
ENTRYPOINT ["/nginx-entrypoint.sh"]

CMD ["nginx"]
