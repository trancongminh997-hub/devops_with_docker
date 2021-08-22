The command used to complete the exercise
```
# build image
docker build . -t spring

# run a container
docker run -it -p 8080:8080 --name spring1 spring
```