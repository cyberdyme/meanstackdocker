
Make sure you are in the mean_docker/angular-client directory, then build your image.

```console
cd angular-client
docker build -t angular-client:dev .
```

Now that the image is built, we can run a container based on that image.
The -d flag tells docker to run the container in detached mode. Meaning, it will run and get you back to your host, without going into the container.

```console
docker run -d --name angular-client -p 4200:4200 angular-client:dev
```

Stop the docker container
```
docker stop angular-client
```
