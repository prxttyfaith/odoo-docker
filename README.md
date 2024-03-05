
#Odoo Docker

## Dependencies of running Odoo on MacOS

###Install docker

```https://docs.docker.com/desktop/install/mac-install/```

### Install docker-compose

``` sudo -i
curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
docker compose version
```

### Git clone

```
git clone https://github.com/prxttyfaith/odoo-docker.git
cd odoo-docker/
```

### cp odoo_pg_pass.example odoo_pg_pass
```
optional: change the value in odoo_pg_pass
```

### Build and run Odoo on docker using docker compose
```
docker-compose up -d
```

```
Visit:
- http://localhost:8069
```

----------------------------------------------------
### Start docker container services
```
docker-compose start
```

### Restart docker container services
```
docker-compose restart
```

### Check the running docker containers
```
docker-compose ps -a
```

### Stop docker container services
```
docker-compose stop
```

----------------------------------------------------
### !DANGER! Remove all the docker containers
```
docker-compose down
```