FROM httpd:latest

# Копируем ваш кастомный конфиг Apache в контейнер
COPY ./config/apache/apache.conf /usr/local/apache2/conf/extra/apache.conf

# Добавляем строку Include в основной конфиг для использования кастомного конфига
RUN echo "Include conf/extra/apache.conf" >> /usr/local/apache2/conf/httpd.conf

# Открываем порт 80 для доступа
EXPOSE 80

# Команда для запуска Apache
CMD ["httpd-foreground"]
