# docker-compose-service

## Products

### Docker

```bash
$ docker-compose up --force-recreate -d
Recreating dockercomposeservice_products-service_1 ...
Recreating dockercomposeservice_products-service_1 ... done
Recreating dockercomposeservice_products-website_1 ...
Recreating dockercomposeservice_products-website_1 ... done
$ docker ps
CONTAINER ID        IMAGE                                   COMMAND                  CREATED             STATUS              PORTS                   NAMES
686a06257367        php:7.0-apache                          "docker-php-entryp..."   10 seconds ago      Up 7 seconds        0.0.0.0:5000->80/tcp    dockercomposeservice_products-website_1
6654d30d3836        dockercomposeservice_products-service   "python api.py"          12 seconds ago      Up 10 seconds       0.0.0.0:5001->80/tcp    dockercomposeservice_products-service_1
```
### Products Service

#### http://localhost:5001
![Products Service](https://github.com/jefftune/docker-compose-service/raw/master/img/products_service_localhost_5001.png)

### Products Website

#### http://localhost:5000
![Products Website](https://github.com/jefftune/docker-compose-service/raw/master/img/products_website_localhost_5000.png)
