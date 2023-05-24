FROM ubuntu:latest

# Установка Apache2
RUN apt-get update && apt-get install -y apache2

# Копирование конфигурационных файлов Apache2
#COPY apache2.conf /etc/apache2/apache2.conf
COPY mywebsite.conf /etc/apache2/sites-available/mywebsite.conf

# Активируем виртуальный хост
RUN a2ensite mywebsite.conf

EXPOSE 80

#Запуска Apache при запуске контейнера
CMD ["apachectl", "-D", "FOREGROUND"]