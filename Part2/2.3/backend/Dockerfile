FROM golang:1.16
WORKDIR /usr/src/myapp
ENV PORT 8080
ENV REQUEST_ORIGIN http://localhost:5000
RUN curl -sL https://github.com/docker-hy/material-applications/archive/main.tar.gz | tar -xz --strip=2 material-applications-main/example-backend
RUN go build
CMD [ "./server"]
