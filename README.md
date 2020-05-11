# PowerDNS 

> docsify serve ./docs


```
docker run -d -p 53:53 -p 53:53/udp --name pdns \
  -e PDNS_api=yes \
  -e PDNS_webserver=yes \
  -e PDNS_webserver_address=0.0.0.0 \
  -e PDNS_webserver_password=123456 \
  -e PDNS_default_ttl=1500 \
  -e PDNS_gmysql_host=10.10.16.160 \
  -e PDNS_gmysql_port=3306 \
  -e PDNS_gmysql_user=root \
  -e PDNS_gmysql_password=1723 \
  -e PDNS_gmysql_dbname=pdns \
  pschiffe/pdns-mysql
```


https://hub.docker.com/r/pschiffe/pdns-admin-uwsgi

https://github.com/ngoduykhanh/PowerDNS-Admin