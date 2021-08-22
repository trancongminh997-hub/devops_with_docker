Commands to run the container
```
# build brand new image
docker build . -t curler

# run the container
docker run --rm -it --name curler1 curler
```
Enter `helsinki.fi` as input. Output matches the 1.4 one
```
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="https://www.helsinki.fi/">here</a>.</p>
</body></html>
```