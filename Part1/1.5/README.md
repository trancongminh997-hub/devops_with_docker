Compare the image sizes between `devopsdockeruh/simple-web-service:ubuntu` and `devopsdockeruh/simple-web-service:alpine`
```
# docker images
REPOSITORY                          TAG       IMAGE ID       CREATED        SIZE
ubuntu                              latest    1318b700e415   3 weeks ago    72.8MB
devopsdockeruh/simple-web-service   ubuntu    4e3362e907d5   5 months ago   83MB
devopsdockeruh/simple-web-service   alpine    fd312adc88e0   5 months ago   15.7MB
```
Commands to check secret message inside alpine container
```
docker run -d --name simple_alpine devopsdockeruh/simple-web-service:alpine

docker exec -it simple_alpine sh

tail -f text.log
```
Secret message is: `You can find the source code here: https://github.com/docker-hy`