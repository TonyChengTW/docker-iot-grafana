# The official Grafana docker image

## Running your Grafana image
download docker image:
```
docker pull grafana/grafana
```



## Configuring  Grafana container

All options defined in conf/grafana.ini can be overriden using environment variables, for example:
Start Docker
```
docker run -id --restart always --name grafana -p 3000:3000 \
  -e "GF_SERVER_ROOT_URL=http://www.strongniche.com.tw"  \
  -e "GF_SECURITY_ADMIN_PASSWORD=1qaz@WSX"  \
  grafana/grafana
```
