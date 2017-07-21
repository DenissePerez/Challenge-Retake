Cloud provider: AWS

Instances: Private IP    -      Public DNS
           172.31.25.33  - ec2-54-200-240-43.us-west-2.compute.amazonaws.com
           172.31.29.52  - ec2-54-201-7-187.us-west-2.compute.amazonaws.com           
           172.31.16.75  - ec2-54-186-200-156.us-west-2.compute.amazonaws.com
           172.31.30.36  - ec2-34-212-26-38.us-west-2.compute.amazonaws.com

CentOs 7

80 Gb of capacity and 30 GB of Memory

yum repolist enabled
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirrors.xmission.com
 * extras: linux.mirrors.es.net
 * updates: mirrors.kernel.org
repo id                      repo name                                    status
base/7/x86_64                CentOS-7 - Base                              9,363
cloudera-manager             Cloudera Manager, Version 5.11.1                 7
extras/7/x86_64              CentOS-7 - Extras                              449
updates/7/x86_64             CentOS-7 - Updates                           2,130
repolist: 11,949




sudo su
[root@ip-172-31-29-52 centos]# useradd -u 2800 saturn
[root@ip-172-31-29-52 centos]# useradd -u 2900 haley
[root@ip-172-31-29-52 centos]# groupadd comets
[root@ip-172-31-29-52 centos]# groupadd planets
[root@ip-172-31-29-52 centos]# usermod -g comets haley
[root@ip-172-31-29-52 centos]# usermod -g planets saturn
[root@ip-172-31-29-52 centos]# ls /etc/passwd | grep saturn
[root@ip-172-31-29-52 centos]# ls /etc/passwd
/etc/passwd
[root@ip-172-31-29-52 centos]# vi /etc/passwd
[root@ip-172-31-29-52 centos]# cat /etc/passwd | grep "saturn"
saturn:x:2800:2902::/home/saturn:/bin/bash
[root@ip-172-31-29-52 centos]# cat /etc/passwd | grep "haley"
haley:x:2900:2901::/home/haley:/bin/bash
[root@ip-172-31-29-52 centos]# cat /etc/gro | grep "haley"
groff/  group   group-
[root@ip-172-31-29-52 centos]# cat /etc/group | grep "comets"
comets:x:2901:
[root@ip-172-31-29-52 centos]# cat /etc/group | grep "planets"
planets:x:2902:
