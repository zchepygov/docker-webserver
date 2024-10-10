FROM php:8.2-fpm

# Копируем кастомный php.ini в контейнер
COPY ./config/php/php.ini /usr/local/etc/php/php.ini

# Устанавливаем необходимые пакеты (например, mysqli, pdo и др.)
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Команда для запуска PHP-FPM
CMD ["php-fpm"]
