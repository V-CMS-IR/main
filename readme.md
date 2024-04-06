# development 

to start working on development you must enter this code

## start all services
```shell
docker compose --env-file=resource-service/.env --env-file=users-service/.env up -d
```


## start users services 

```shell
docker compose --env-file=users-service/.env up users-service-db users-service  -d
```

NOTE : to working with users-service you don't need to complete the resource-service env  
