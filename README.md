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


## Assignment

1. Create a dockerfile to run server.rb
2. Create a dockerfile to run client.rb
3. Build and start server and client, make sure the client sends request to server sucessfully
4. Create a docker-compose file to start 5 clients and 1 server