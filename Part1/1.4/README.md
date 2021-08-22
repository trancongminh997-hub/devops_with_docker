The command used to start process:
```
docker run --rm -it --name missdep ubuntu sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
```
A problem is that `curl` is not available.

The command used to fix the ensuing problems:
```
docker run --rm -it --name missdep ubuntu sh -c 'apt-get update; apt-get install curl -y; echo 
"Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
```

Another problem is that it does not wait for inputs quite interactively

Finally this command works
```
docker run --rm -it -a STDIN -a STDOUT -a STDERR --name missdep ubuntu sh -c 'apt-get update; apt-get install curl -y; echo 
"Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
```
