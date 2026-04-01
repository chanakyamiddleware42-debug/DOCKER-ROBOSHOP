FROM nginx:1.24
RUN rm -f /usr/share/nginx/html/* 
COPY frontend-v3/* /usr/share/nginx/html/
RUN rm -f  /etc/nginx/nginx.conf
COPY nginx.conf /etc/nginx/
CMD ["nginx","-g", "daemon off;"]
