FROM jerfeson/npf:php73

#Default operating system settings
RUN ln -f -s /usr/share/zoneinfo/America/Sao_Paulo /etc/localtime

#Configuring Redis to register sessions
RUN echo "[Session]" >> /etc/php/7.3/fpm/php.ini
RUN echo "session.save_handler = redis" >> /etc/php/7.3/fpm/php.ini
RUN echo "session.save_path = tcp://redis:6379" >> /etc/php/7.3/fpm/php.ini