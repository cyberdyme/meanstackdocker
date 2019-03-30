Create dock and start it

```cmd
docker build -t express-server:dev .
docker run -d --name express-server -p 3000:3000 express-server:dev
```

Stop the docker
```cmd
 docker stop express-server
```