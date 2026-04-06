FROM nginx:1.24.0

RUN rm -f /usr/share/nginx/html/index.html
RUN rm -f /etc/nginx/nginx.conf
RUM rm -f /etc/nginx/conf.d/default.conf

COPY nginx.conf /etc/nginx/nginx.conf
COPY static /usr/share/nginx/html/

CMD ["nginx", "-g", "daemon off;"]

# then run using `docker run -d -p 80:80 --network roboshop --name frontend frontend:1.0.0`