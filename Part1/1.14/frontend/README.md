Make sure current directory is relatively `/material-applications/example-frontend`

```docker build . -t hello_frontend:1.12```

```docker run -d -p 5000:5000 --name cuti hello_frontend:1.12```

Navigate to  `localhost:5000` on browser, click on button for 1.14, the result euivalent to following:<br>
![alt text](https://github.com/trancongminh997-hub/devops_with_docker/blob/main/Part1/1.14/backend/Screenshot_1_14.jpg?raw=true)
