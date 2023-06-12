### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## Docker

Build sigma docker image:
```
docker build . -f D:\develop\vue_primevue_template\public\Dockerfile -t containers.orel.in/zkh-online-front:0.0.1
```

Run docker image (navigate to http://localhost:8080/):
```
docker run -d -p 8080:8080 --rm --name zkh-online-front containers.orel.in/zkh-online-front:0.0.1
```

Run sigma docker image in dev mode:
```
docker run -it -p 8080:8080 -v .:/app --rm --entrypoint="/dev.sh" --name zkh-online-front containers.orel.in/zkh-online-front:0.0.1
```