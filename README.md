docker-phabricator
==================
Dockerfile with debian:jessie / apache2 / mysql / phabricator


Run
----
```
docker run arep/docker-phabricator
```

Build and run
---------------

```
git clone https://github.com/arep/docker-phabricator.git
./build.sh
./run-server.sh
````

Go to http://localhost.local:8081

Docker HTTP listen on 8081 and ssh listen on 2244

You can connect with ssh with this command (and password docker): 
```
ssh admin@localhost -p 2244
```

Mysql files are written on `/data/phabricator/mysql` (described in run-server.sh)

Conf files are written on `/data/phabricator/conf` (described in run-server.sh)

Repositories files are written on `/data/phabricator/repo` (described in run-server.sh)

