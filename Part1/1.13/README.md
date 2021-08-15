Make sure current directory is relatively `/material-applications/example-backend`

```docker build . -t hello_backend:1.16```
```docker run --rm -it -p 8080:8080 --name cuti2 hello_backend:1.16```

Navigate to  `http://localhost:8080/ping` on browser, you should get a `pong` as response.
