Este repositorio alberga los archivos Docker Compose de CTFd y NGINX Proxy. Este último añade el certificado SSL proporcionado por el contenedor NGINX Proxy, modificando así el archivo Docker Compose de CTFd. 


Install

```
cd CTFd
```

```
docker-compose up -d
```

```
cd nginx-proxy
```

```
docker-compose up -d
```
