FROM base/archlinux

RUN pacman -Sy

RUN echo "Y" | pacman -S mariadb

RUN useradd mysql

RUN mysql_install_db --user=mysql --basedir=/usr --datadir=/var/lib/mysql

USER mysql

RUN mysqld
