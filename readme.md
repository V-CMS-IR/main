# development 

to start working on development you must enter this code

#### then need to create private key and extract pub key from it 
```bash
   mkdir secrets && 
   openssl genrsa -out ./secrets/cms_private.pem 2048 && 
   openssl rsa -in ./secrets/cms_private.pem -pubout -out ./secrets/cms_public.pem
```
## start all services
```shell
docker compose --env-file=resource-service/.env --env-file=users-service/.env --env-file=./.env up -d
```


## start users services 

```shell
docker compose --env-file=users-service/.env --env-file=./.env up users-service-db users-service  -d
```

NOTE : to working with users-service you don't need to complete the resource-service env  
