2017-08-04 13:22:02,883 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.11.1 (#9 built by jenkins on 20170525-1411 git: 8adcfb8545cb0a35f590717b2626a9ea04948dae) 2017-08-04 15:12:02,957 INFO main:org.mortbay.log: Logging to org.slf4j.impl.Log4jLoggerAdapter(org.mortbay.log) via org.mortbay.log.Slf4jLog 2017-08-04 15:12:03,079 INFO main:org.springframework.context.support.ClassPathXmlApplicationContext: Refreshing org.springframework.context.support.ClassPathXmlApplicationContext@35b4e829: startup date [Fri Aug 4 15:12:03 UTC 2017]; root of context hierarchy

2017-08-04 13:32:57,836 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.






It contains the database connection, host, name, user  and type.
Currently 'mysql', 'postgresql' and 'oracle' are valid databases.com.cloudera.cmf.db.type=mysql

If a non standard port is needed, use 'hostname:port'com.cloudera.cmf.db.host=ip-172-31-29-52:3306
The database name

com.cloudera.cmf.db.name=scm
The database user

com.cloudera.cmf.db.user=root
The database user's password

com.cloudera.cmf.db.password=1234
The db setup type
By default, it is set to INIT
If scm-server uses Embedded DB then it is set to EMBEDDED
If scm-server uses External DB then it is set to EXTERNAL

com.cloudera.cmf.db.setupType=EXTERNAL
