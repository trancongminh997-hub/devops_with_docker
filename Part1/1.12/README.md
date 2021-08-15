Make sure current directory is relatively `/material-applications/example-frontend`

```docker build . -t hello_frontend:1.12```

```docker run --rm -it -p 5000:5000 --name cuti hello_frontend:1.12```

Navigate to  `localhost:5000` on browser, the result euivalent to following:<br>
![alt text](https://github.com/trancongminh997-hub/devops_with_docker/blob/main/Part1/1.12/Screenshot_1_12.jpg?raw=true)
