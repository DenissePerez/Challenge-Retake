
sudo yum install mariadb-server
sudo service mariadb stop
cd /etc
vi my.cnf

sudo systemctl enable mariadb 
sudo systemctl list-unit-files | grep mariadb

sudo service mariadb start
/usr/bin/mysql_secure_installation
mkdir -p /usr/share/java/
#subir archivos mysql

mysql -u root -p

create database amon DEFAULT CHARACTER SET utf8;
grant all on amon.* TO 'amon'@'%' IDENTIFIED BY 'amon_password';

create database rman DEFAULT CHARACTER SET utf8;
grant all on rman.* TO 'rman'@'%' IDENTIFIED BY 'rman_password';

create database metastore DEFAULT CHARACTER SET utf8;
grant all on metastore.* TO 'hive'@'%' IDENTIFIED BY 'hive_password';

create database sentry DEFAULT CHARACTER SET utf8;
grant all on sentry.* TO 'sentry'@'%' IDENTIFIED BY 'sentry_password';

create database nav DEFAULT CHARACTER SET utf8;
grant all on nav.* TO 'nav'@'%' IDENTIFIED BY 'nav_password';

create database navms DEFAULT CHARACTER SET utf8;
grant all on navms.* TO 'navms'@'%' IDENTIFIED BY 'navms_password';

create database hue DEFAULT CHARACTER SET utf8;
grant all on hue.* TO 'hue'@'%' IDENTIFIED BY 'hue_password';

create database oozie DEFAULT CHARACTER SET utf8;
grant all on oozie.* TO 'oozie'@'%' IDENTIFIED BY 'oozie_password';

create database cms DEFAULT CHARACTER SET utf8;
grant all on cms.* TO 'cms'@'%' IDENTIFIED BY 'cms';

create database cmf DEFAULT CHARACTER SET utf8;
grant all on cmf.* TO 'cmf'@'%' IDENTIFIED BY 'cmf';

[root@ip-172-31-22-184 etc]# hostname
ip-172-31-22-184
[root@ip-172-31-22-184 etc]# yum list installed | grep mariadb
mariadb.x86_64                  1:5.5.52-1.el7                 @base
mariadb-libs.x86_64             1:5.5.52-1.el7                 @base
mariadb-server.x86_64           1:5.5.52-1.el7                 @base
[root@ip-172-31-22-184 etc]# mysql -uroot -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 12
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| cmf               |
| cms                |
| hue                |
| metastore          |
| mysql              |
| nav                |
| navms              |
| oozie              |
| performance_schema |
| rman               |
| sentry             |
+--------------------+
12 rows in set (0.00 sec)
 mysql -uroot -p Server version: 5.5.52-MariaDB MariaDB Server

MariaDB [(none)]> show databases; +--------------------+ | Database | +--------------------+ | information_schema | | amon | | hue | | metastore | | mysql | | nav | | navms | | oozie | | performance_schema | | rman | | scm | | sentry | +--------------------+ 12 rows in set (0.00 sec)
