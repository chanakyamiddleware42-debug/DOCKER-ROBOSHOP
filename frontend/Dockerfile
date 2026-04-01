FROM nginx:1.24
RUN rm -f /usr/share/nginx/html/index.html
RUN rm -f /etc/nginx/nginx.conf
RUN rm -f /etc/nginx/conf.d/*.conf
COPY frontend-v3 /usr/share/nginx/html/
COPY nginx.conf /etc/nginx/nginx.conf
#CMD ["nginx","-g", "daemon off;"]
