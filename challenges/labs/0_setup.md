Cloud provider: AWS

Instances: Private IP    -      Public DNS

           172.31.22.184  - ec2-54-202-159-209.us-west-2.compute.amazonaws.com
           
           172.31.17.168  - ec2-54-213-238-242.us-west-2.compute.amazonaws.com 
           
           172.31.17.22  -  ec2-54-218-72-196.us-west-2.compute.amazonaws.com
           
           172.31.27.20  -  ec2-54-245-152-67.us-west-2.compute.amazonaws.com
           
           

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
[root@ip-172-31-22-184 ~]# useradd -u 2800 saturn

[root@ip-172-31-22-184 ~]# useradd -u 2900 haley

[root@ip-172-31-22-184 ~]# groupadd comets

[root@ip-172-31-22-184 ~]# groupadd planets

[root@ip-172-31-22-184 ~]# usermod -g comets haley

[root@ip-172-31-22-184 ~]# usermod -g planets saturn

[root@ip-172-31-22-184 ~]# ls /etc/passwd | grep saturn

[root@ip-172-31-22-184 ~]# ls /etc/passwd

/etc/passwd

[root@ip-172-31-22-184 ~]# vi /etc/passwd

saturn:x:2800:2902::/home/saturn:/bin/bash

haley:x:2900:2901::/home/haley:/bin/bash


[root@ip-172-31-22-184 ~]# cat /etc/passwd | grep "saturn"

saturn:x:2800:2902::/home/saturn:/bin/bash


[root@ip-172-31-22-184 ~]# cat /etc/passwd | grep "haley"

haley:x:2900:2901::/home/haley:/bin/bash

[root@ip-172-31-22-184 ~]# cat /etc/gro | grep "haley"

groff/  group   group-

[root@ip-172-31-22-184 ~]# cat /etc/group | grep "comets"

comets:x:2901:

[root@ip-172-31-22-184 ~]# cat /etc/group | grep "planets"

planets:x:2902:

