#Use specific nginx version
FROM nginx:1.15.5

#Remove the main nginx config
RUN rm /etc/nginx/nginx.conf

#Put our custom nginx config in its place
COPY nginx.conf /etc/nginx/

#Remove any existing site configs
RUN rm /etc/nginx/conf.d/*.conf

#Put our website specific config
COPY my_web_app.conf /etc/nginx/conf.d/
