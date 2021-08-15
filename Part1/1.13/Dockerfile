FROM golang:1.16
WORKDIR /usr/src/myapp
COPY . /usr/src/myapp
RUN go build
EXPOSE 8080
CMD [ "./server"]
