ls /etc/yum.repos.d


CentOS-Base.repo       CentOS-fasttrack.repo  CentOS-Vault.repo

CentOS-CR.repo         CentOS-Media.repo      cloudera-manager.repo

CentOS-Debuginfo.repo  CentOS-Sources.repo



yum list installed | grep cloudera

cloudera-manager-agent.x86_64   5.11.1-1.cm5111.p0.9.el7       @cloudera-manager

cloudera-manager-daemons.x86_64 5.11.1-1.cm5111.p0.9.el7       @cloudera-manager

jdk.x86_64                      2000:1.6.0_31-fcs              @cloudera-manager

oracle-j2sdk1.7.x86_64          1.7.0+update67-1               @cloudera-manager
