FROM registry.dev.own3d.tv/ghostzero/sailor:latest

ARG WWWGROUP

COPY . /var/www/html

RUN composer install --ignore-platform-reqs

# Make the php user owner of the directory
RUN chmod -R 777 storage bootstrap database
#RUN chown -R $WWWGROUP:$WWWGROUP storage bootstrap database
