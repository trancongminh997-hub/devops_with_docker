The command used to complete the exercise
```
# need to create a file beforehand
touch text.log

# run a container
docker run -it -v  "$(pwd)/text.log:/usr/src/app/text.log" --name vol19 devopsdockeruh/simple-web-service:ubuntu
```
Check file `text.log` in current directory for sample content