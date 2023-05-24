FROM nginx:latest

# Удаляем стандартную кофигурацию Nginx
RUN rm /etc/nginx/conf.d/default.conf

# Копируемый файл кофигурации Nginx
COPY mywebsite.conf /etc/nginx/conf.d/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]