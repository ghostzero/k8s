FROM registry.dev.own3d.tv/ghostzero/sailor:latest

COPY . /var/www/html

RUN composer install --ignore-platform-reqs

# Make the php user owner of the directory
RUN chmod -R 755 storage bootstrap database
RUN chown -R www-data:www-data storage bootstrap database
