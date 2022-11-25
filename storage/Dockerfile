FROM nginx:latest
RUN chmod 777 -R /etc/nginx/conf.d/
RUN chmod 777 -R /usr/share/nginx/html 
COPY default.conf /etc/nginx/conf.d/default.conf
RUN ls /etc/nginx/conf.d/
COPY site-content /usr/share/nginx/html
RUN ls /usr/share/nginx/html
EXPOSE 80
ENTRYPOINT ["nginx","-g","daemon off;"]
