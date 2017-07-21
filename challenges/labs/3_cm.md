

hdfs hdfs dfs -ls /user/ Found 7 items drwxr-xr-x - hdfs supergroup 0 2017-07-21 14:29 /user/haley drwxrwxrwx - mapred hadoop 0 2017-07-21 14:23 /user/history drwxrwxr-t - hive hive 0 2017-07-21 14:24 /user/hive drwxrwxr-x - hue hue 0 2017-07-21 14:24 /user/hue drwxrwxr-x - oozie oozie 0 2017-07-21 14:24 /user/oozie drwxr-xr-x - hdfs supergroup 0 2017-07-21 14:29 /user/saturn drwxr-x--x - spark spark 0 2017-07-21 14:23 /user/spark

../api/v14/hosts

{ "items": [ { "hostId": "0704efac-44d9-4cc2-86fb-594b8504eb9b", "ipAddress": "172.31.25.33", "hostname": "ip-172-31-25-33.ec2.internal", "rackId": "/default", "hostUrl": 
"http://ip-172-31-29-52.ec2.internal:7180/cmf/hostRedirect/0704efac-44d9-4cc2-86fb-594b8504eb9b", "maintenanceMode": false, 
"maintenanceOwners": [], "commissionState": "COMMISSIONED", "numCores": 8, "numPhysicalCores": 4, 
"totalPhysMemBytes": 33299312640 }, { "hostId": "1a26cb5f-6662-4c00-862a-5444bea612d5", "ipAddress": "172.31.16.75", 
"hostname": "ip-172-31-16-75.ec2.internal", "rackId": "/default", "hostUrl":
"http://ip-172-31-29-52.ec2.internal:7180/cmf/hostRedirect/1a26cb5f-6662-4c00-862a-5444bea612d5", "maintenanceMode": false, 
"maintenanceOwners": [], "commissionState": "COMMISSIONED", "numCores": 8, "numPhysicalCores": 4, "totalPhysMemBytes": 
33299312640 }, { "hostId": "b4bbb83a-2d22-4e94-ba09-d6d3b200e954", "ipAddress": "172.31.29.52", "hostname": 
"ip-172-31-29-52.ec2.internal", "rackId": "/default", "hostUrl": "http://ip-172-31-29-52.ec2.internal:7180/cmf/hostRedirect/
b4bbb83a-2d22-4e94-ba09-d6d3b200e954", "maintenanceMode": false, "maintenanceOwners": [], "commissionState": 
"COMMISSIONED", "numCores": 8, "numPhysicalCores": 4, "totalPhysMemBytes": 33299312640 }, 
{ "hostId": "d263a074-491d-4330-8c18-2b9ee4c198f4", "ipAddress": "172.31.30.36", "hostname": "ip-172-31-30-36.ec2.internal", 
"rackId": "/default", "hostUrl": "http://ip-172-31-29-52.ec2.internal:7180/cmf/hostRedirect/d263a074-491d-4330-8c18-2b9ee4c198f4",
"maintenanceMode": false, "maintenanceOwners": [], "commissionState": "COMMISSIONED", "numCores": 8, "numPhysicalCores": 4, 
"totalPhysMemBytes": 33299312640 } ] }

/api/v8/clusters//services

{ "items": [ { "name": "hive", "type": "HIVE", "clusterRef": { "clusterName": "cluster" }, "serviceUrl": 
"http://ip-172-31-29-52.ec2.internal:7180/cmf/serviceRedirect/hive", "serviceState": "STARTED", "healthSummary": "GOOD", 
"healthChecks": [ { "name": "HIVE_HIVEMETASTORES_HEALTHY", "summary": "GOOD" }, { "name": "HIVE_HIVESERVER2S_HEALTHY", "summary":
"GOOD" } ], "configStalenessStatus": "FRESH", "clientConfigStalenessStatus": "FRESH", "maintenanceMode": false,
"maintenanceOwners": [], "displayName": "Hive" }, { "name": "zookeeper", "type": "ZOOKEEPER", "clusterRef": 
{ "clusterName": "cluster" }, "serviceUrl": "http://ip-172-31-29-52.ec2.internal:7180/cmf/serviceRedirect/zookeeper", 
"serviceState": "STARTED", "healthSummary": "GOOD", "healthChecks": [ { "name": "ZOOKEEPER_CANARY_HEALTH", "summary": "GOOD" }, 
{ "name": "ZOOKEEPER_SERVERS_HEALTHY", "summary": "GOOD" } ], "configStalenessStatus": "FRESH", "clientConfigStalenessStatus": 
"FRESH", "maintenanceMode": false, "maintenanceOwners": [], "displayName": "ZooKeeper" }, { "name": "hue", "type": "HUE",
"clusterRef": { "clusterName": "cluster" }, "serviceUrl": "http://ip-172-31-29-52.ec2.internal:7180/cmf/serviceRedirect/hue", 
"serviceState": "STARTED", "healthSummary": "GOOD", "healthChecks": [ { "name": "HUE_HUE_SERVERS_HEALTHY", "summary": "GOOD" } ],
"configStalenessStatus": "FRESH", "clientConfigStalenessStatus": "FRESH", "maintenanceMode": false, "maintenanceOwners": [], 
"displayName": "Hue" }, { "name": "oozie", "type": "OOZIE", "clusterRef": { "clusterName": "cluster" }, "serviceUrl":
"http://ip-172-31-29-52.ec2.internal:7180/cmf/serviceRedirect/oozie", "serviceState": "STARTED", "healthSummary": "GOOD", 
"healthChecks": [ { "name": "OOZIE_OOZIE_SERVERS_HEALTHY", "summary": "GOOD" } ], "configStalenessStatus": "FRESH", 
"clientConfigStalenessStatus": "FRESH", "maintenanceMode": false, "maintenanceOwners": [], "displayName": "Oozie" }, 
{ "name": "yarn", "type": "YARN", "clusterRef": { "clusterName": "cluster" }, "serviceUrl": "http://ip-172-31-29-52.ec2.internal:
7180/cmf/serviceRedirect/yarn", "serviceState": "STARTED", "healthSummary": "GOOD", "healthChecks": [ { "name": 
"YARN_JOBHISTORY_HEALTH", "summary": "GOOD" }, { "name": "YARN_NODE_MANAGERS_HEALTHY", "summary": "GOOD" }, { "name": 
"YARN_RESOURCEMANAGERS_HEALTH", "summary": "GOOD" }, { "name": "YARN_USAGE_AGGREGATION_HEALTH", "summary": "DISABLED" } ], 
"configStalenessStatus": "FRESH", "clientConfigStalenessStatus": "FRESH", "maintenanceMode": false, "maintenanceOwners": [],
"displayName": "YARN (MR2 Included)" }, { "name": "spark_on_yarn", "type": "SPARK_ON_YARN", "clusterRef": { "clusterName": "
cluster" }, "serviceUrl": "http://ip-172-31-29-52.ec2.internal:7180/cmf/serviceRedirect/spark_on_yarn", "serviceState": 
"STARTED", "healthSummary": "GOOD", "healthChecks": [], "configStalenessStatus": "FRESH", "clientConfigStalenessStatus": 
"FRESH", "maintenanceMode": false, "maintenanceOwners": [], "displayName": "Spark" }, { "name": "hdfs", "type": "HDFS", "
clusterRef": { "clusterName": "cluster" }, "serviceUrl": "http://ip-172-31-29-52.ec2.internal:7180/cmf/serviceRedirect/hdfs", 
"serviceState": "STARTED", "healthSummary": "GOOD", "healthChecks": [ { "name": "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS", "summary":
"GOOD" }, { "name": "HDFS_CANARY_HEALTH", "summary": "GOOD" }, { "name": "HDFS_DATA_NODES_HEALTHY", "summary": "GOOD" }, {
"name": "HDFS_FREE_SPACE_REMAINING", "summary": "GOOD" }, { "name": "HDFS_HA_NAMENODE_HEALTH", "summary": "GOOD" }, 
{ "name": "HDFS_MISSING_BLOCKS", "summary": "GOOD" }, { "name": "HDFS_UNDER_REPLICATED_BLOCKS", "summary": "GOOD" } ]
, "configStalenessStatus": "FRESH", "clientConfigStalenessStatus": "FRESH", "maintenanceMode": false, "maintenanceOwners":
[], "displayName": "HDFS" } ] }
