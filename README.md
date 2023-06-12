### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## Docker

Build sigma docker image:
```
docker build . -t containers.orel.in/zkh-online-front:0.0.1
docker build . -f Dockerfile -t containers.orel.in/zkh-online-front:0.0.1
docker run --rm -it containers.orel.in/zkh-online-front:0.0.1
```

Run sigma docker image (navigate to http://localhost:8080/):
```
docker run -it -p 8080:8080 --rm --name sigma containers.orel.in/sigma:0.0.1
```

Run sigma docker image in dev mode:
```
docker run -it -p 8080:8080 -v $PWD:/app --rm --entrypoint="/dev.sh" --name sigma containers.orel.in/sigma:0.0.1
```