create jenkins network

```
echo "docker network create jenkins" >> README.md
```

start docker:bind container

```
# chmod +x start-dockerdind
./start-dockerdind
```

build jenkins container

```
docker build -f Dockerfile-local -t myjenkins-blueocean:2.452.2-1 .
```

run a jenkins container with the newly created image

```
# chmod +x start-localjenkins
./start-localjenkins
```

Accessing jenkins container throug command line

```
docker exec -it jenkins-blueocean bash
```

