FROM nginx:alpine

COPY index.html /usr/share/nginx/html/index.html

RUN sed -i 's/listen 80;/listen 8080;/g' /etc/nginx/conf.d/default.conf

ENV PORT 8080

CMD ["sh", "-c", "nginx -g 'daemon off;'"]
