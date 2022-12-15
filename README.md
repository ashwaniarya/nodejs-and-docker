# nodejs-and-docker



## Run these command step by step

```bash
$ docker build . -t nodejs-and-docker
```

Here -t means tag name and we will use same tag for status and deployment.

### To check the details of docker image we just built

```{bash}
$ docker images

REPOSITORY          TAG              IMAGE ID       CREATED         SIZE
nodejs-and-docker   latest           9d23e64b868f   3 minutes ago   176MB
```

### Now we will test it locally
```bash
$ docker run -p 1337:1337 nodejs-and-docker
```

Now mode to http://localhost:1337/status
