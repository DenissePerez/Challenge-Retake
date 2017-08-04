[root@ip-172-31-17-168 yum.repos.d]# curl -X POST -v -u 'admin:admin' http://localhost:7180/api/v17/clusters/DenissePerez/services/hive/commands/stop
* About to connect() to localhost port 7180 (#0)
*   Trying ::1...
* Connection refused
*   Trying 127.0.0.1...
* Connected to localhost (127.0.0.1) port 7180 (#0)
* Server auth using Basic with user 'admin'
> POST /api/v17/clusters/DenissePerez/services/hive/commands/stop HTTP/1.1
> Authorization: Basic YWRtaW46YWRtaW4=
> User-Agent: curl/7.29.0
> Host: localhost:7180
> Accept: */*
>
< HTTP/1.1 200 OK
< Expires: Thu, 01-Jan-1970 00:00:00 GMT
< Set-Cookie: CLOUDERA_MANAGER_SESSIONID=84m6zvzbin521166cepbaznl8;Path=/;HttpOnly
< Content-Type: application/json
< Date: Fri, 04 Aug 2017 20:54:06 GMT
< Transfer-Encoding: chunked
< Server: Jetty(6.1.26.cloudera.4)
<
{
  "id" : 393,
  "name" : "Stop",
  "startTime" : "2017-08-04T20:54:06.897Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
* Connection #0 to host localhost left intact





}[root@ip-172-31-17-168 yum.repos.d]# curl -X POST -v -u 'admin:admin' http://localhost:7180/api/v17/clusters/DenissePerez/services/hive/ommands/start
* About to connect() to localhost port 7180 (#0)
*   Trying ::1...
* Connection refused
*   Trying 127.0.0.1...
* Connected to localhost (127.0.0.1) port 7180 (#0)
* Server auth using Basic with user 'admin'
> POST /api/v17/clusters/DenissePerez/services/hive/commands/start HTTP/1.1
> Authorization: Basic YWRtaW46YWRtaW4=
> User-Agent: curl/7.29.0
> Host: localhost:7180
> Accept: */*
>
< HTTP/1.1 200 OK
< Expires: Thu, 01-Jan-1970 00:00:00 GMT
< Set-Cookie: CLOUDERA_MANAGER_SESSIONID=t5c4sh7u8t73r5dt7up3j91l;Path=/;HttpOnly
< Content-Type: application/json
< Date: Fri, 04 Aug 2017 20:54:45 GMT
< Transfer-Encoding: chunked
< Server: Jetty(6.1.26.cloudera.4)
<
{
  "id" : 397,
  "name" : "Start",
  "startTime" : "2017-08-04T20:54:45.537Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
* Connection #0 to host localhost left intact
