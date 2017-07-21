ls /etc/yum.repos.d


CentOS-Base.repo       CentOS-fasttrack.repo  CentOS-Vault.repo

CentOS-CR.repo         CentOS-Media.repo      cloudera-manager.repo

CentOS-Debuginfo.repo  CentOS-Sources.repo



yum list installed | grep cloudera

cloudera-manager-agent.x86_64   5.11.1-1.cm5111.p0.9.el7       @cloudera-manager

cloudera-manager-daemons.x86_64 5.11.1-1.cm5111.p0.9.el7       @cloudera-manager

jdk.x86_64                      2000:1.6.0_31-fcs              @cloudera-manager

oracle-j2sdk1.7.x86_64          1.7.0+update67-1               @cloudera-manager


/usr/share/cmf/schema/scm_prepare_database.sh mysql -uroot -p scm scm scm Enter database password: JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera Verifying that we can write to /etc/cloudera-scm-server Creating SCM configuration file in /etc/cloudera-scm-server Executing: /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db. [ main] DbCommandExecutor INFO Successfully connected to database. All done, your SCM database is configured correctly!
