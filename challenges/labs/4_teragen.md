sudo -u saturn hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen 65536000 tgen


17/08/04 17:56:46 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-168.us-west-2.compute.internal/172.31.17.168:8032
17/08/04 17:56:46 INFO terasort.TeraSort: Generating 65536000 using 2
17/08/04 17:56:46 INFO mapreduce.JobSubmitter: number of splits:2
17/08/04 17:56:46 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1501866075416_0001
17/08/04 17:56:47 INFO impl.YarnClientImpl: Submitted application application_1501866075416_0001
17/08/04 17:56:47 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-168.us-west-2.compute.internal:8088/proxy/application_1501866075416_0001/
17/08/04 17:56:47 INFO mapreduce.Job: Running job: job_1501866075416_0001
17/08/04 17:56:53 INFO mapreduce.Job: Job job_1501866075416_0001 running in uber mode : false
17/08/04 17:56:53 INFO mapreduce.Job:  map 0% reduce 0%
17/08/04 17:57:04 INFO mapreduce.Job:  map 11% reduce 0%
17/08/04 17:57:07 INFO mapreduce.Job:  map 16% reduce 0%
17/08/04 17:57:10 INFO mapreduce.Job:  map 19% reduce 0%
17/08/04 17:57:13 INFO mapreduce.Job:  map 22% reduce 0%
17/08/04 17:57:16 INFO mapreduce.Job:  map 25% reduce 0%
17/08/04 17:57:19 INFO mapreduce.Job:  map 28% reduce 0%
17/08/04 17:57:22 INFO mapreduce.Job:  map 31% reduce 0%
17/08/04 17:57:25 INFO mapreduce.Job:  map 33% reduce 0%
17/08/04 17:57:26 INFO mapreduce.Job:  map 34% reduce 0%
17/08/04 17:57:28 INFO mapreduce.Job:  map 37% reduce 0%
17/08/04 17:57:29 INFO mapreduce.Job:  map 39% reduce 0%
17/08/04 17:57:31 INFO mapreduce.Job:  map 42% reduce 0%
17/08/04 17:57:32 INFO mapreduce.Job:  map 45% reduce 0%
17/08/04 17:57:34 INFO mapreduce.Job:  map 46% reduce 0%
17/08/04 17:57:35 INFO mapreduce.Job:  map 47% reduce 0%
17/08/04 17:57:37 INFO mapreduce.Job:  map 49% reduce 0%
17/08/04 17:57:38 INFO mapreduce.Job:  map 50% reduce 0%
17/08/04 17:57:40 INFO mapreduce.Job:  map 52% reduce 0%
17/08/04 17:57:41 INFO mapreduce.Job:  map 53% reduce 0%
17/08/04 17:57:43 INFO mapreduce.Job:  map 54% reduce 0%
17/08/04 17:57:44 INFO mapreduce.Job:  map 56% reduce 0%
17/08/04 17:57:46 INFO mapreduce.Job:  map 57% reduce 0%
17/08/04 17:57:47 INFO mapreduce.Job:  map 59% reduce 0%
17/08/04 17:57:50 INFO mapreduce.Job:  map 61% reduce 0%
17/08/04 17:57:53 INFO mapreduce.Job:  map 64% reduce 0%
17/08/04 17:57:56 INFO mapreduce.Job:  map 67% reduce 0%
17/08/04 17:57:59 INFO mapreduce.Job:  map 70% reduce 0%
17/08/04 17:58:02 INFO mapreduce.Job:  map 73% reduce 0%
17/08/04 17:58:05 INFO mapreduce.Job:  map 76% reduce 0%
17/08/04 17:58:08 INFO mapreduce.Job:  map 78% reduce 0%
17/08/04 17:58:11 INFO mapreduce.Job:  map 81% reduce 0%
17/08/04 17:58:14 INFO mapreduce.Job:  map 84% reduce 0%
17/08/04 17:58:17 INFO mapreduce.Job:  map 87% reduce 0%
17/08/04 17:58:20 INFO mapreduce.Job:  map 89% reduce 0%
17/08/04 17:58:23 INFO mapreduce.Job:  map 92% reduce 0%
17/08/04 17:58:26 INFO mapreduce.Job:  map 95% reduce 0%
17/08/04 17:58:29 INFO mapreduce.Job:  map 98% reduce 0%
17/08/04 17:58:32 INFO mapreduce.Job:  map 99% reduce 0%
17/08/04 17:58:33 INFO mapreduce.Job:  map 100% reduce 0%
17/08/04 17:58:33 INFO mapreduce.Job: Job job_1501866075416_0001 completed successfully
17/08/04 17:58:33 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=247206
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=170
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=8
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=194222
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=194222
                Total vcore-seconds taken by all map tasks=194222
                Total megabyte-seconds taken by all map tasks=198883328
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=624
                CPU time spent (ms)=91030
                Physical memory (bytes) snapshot=408326144
                Virtual memory (bytes) snapshot=3204947968
                Total committed heap usage (bytes)=753401856
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000
                
                
                
   


[root@ip-172-31-17-168 saturn]# sudo -u hdfs hdfs dfs -ls /user/saturn/
Found 1 items
drwxr-xr-x   - saturn supergroup          0 2017-08-04 17:58 /user/saturn/tgen

sudo -u hdfs hadoop fsck -blocks /user/saturn
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-17-168.us-west-2.compute.internal:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.17.168 for path /user/saturn at Fri Aug 04 18:09:56 UTC 2017
...Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    2
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      50 (avg. block size 131072000 B)
 Minimally replicated blocks:   50 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          3
 Number of racks:               1
FSCK ended at Fri Aug 04 18:09:56 UTC 2017 in 3 milliseconds


The filesystem under path '/user/saturn' is HEALTHY



