FROM nginx:alpine

# Copy custom nginx config
COPY ./Angular/nginx.conf /etc/nginx/nginx.conf

COPY ./Angular/datascience/dist/datascience/ /usr/share/nginx/html

EXPOSE 80 443

ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]
