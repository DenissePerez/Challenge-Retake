
hostname ip 172.31.25.33

yum list installed | grep mariadb mariadb.x86_64 1:5.5.52-1.el7 @base

mariadb-libs.x86_64 1:5.5.52-1.el7 @base/7.3.1611

mariadb-server.x86_64 1:5.5.52-1.el7 @base

 mysql -uroot -p Server version: 5.5.52-MariaDB MariaDB Server

MariaDB [(none)]> show databases; +--------------------+ | Database | +--------------------+ | information_schema | | amon | | hue | | metastore | | mysql | | nav | | navms | | oozie | | performance_schema | | rman | | scm | | sentry | +--------------------+ 12 rows in set (0.00 sec)
