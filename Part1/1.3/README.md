
Command
```
# Run a container
docker run -d --rm --name smsg devopsdockeruh/simple-web-service:ubuntu

# Create interactive shell within container
docker exec -it smsg /bin/bash

# follow the logs
tail -f ./text.log
```
Secret message is: `You can find the source code here: https://github.com/docker-hy`