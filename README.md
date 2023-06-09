# docker-ruby

## Docker server
```
docker build -t my-server-app ./server

docker run -p 3333:3333 my-server-app
```

## Docker client
```
docker build -t my-client-app ./client
docker run --network="host" my-client-app
```

## Docker compose
```
docker-compose up
```