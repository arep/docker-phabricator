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

You can connect with this command: 
```
docker-enter phabricator
```
Nsenter (and docker-enter) can be installed like this:
```
docker run --rm -v /usr/local/bin:/target jpetazzo/nsenter
```

Mysql files are written on `/data/phabricator/mysql` (described in run-server.sh)

Conf files are written on `/data/phabricator/conf` (described in run-server.sh)

Repositories files are written on `/data/phabricator/repo` (described in run-server.sh)

