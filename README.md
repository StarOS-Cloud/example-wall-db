# Wall Mysql

It's a mysql image for demo `Wall`。

### Build
```
docker build -t wall/mysql:<TAG> .
```

### Run
```
docker run -d -p 3306:3306 \
  --name wall-mysql \
  -e MYSQL_ROOT_PASSWORD=<PASSWORD> \
  -v <DATADIR>:/var/lib/mysql \
  wall/mysql:<TAG>
```
