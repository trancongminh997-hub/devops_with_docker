FROM golang:1.16
WORKDIR /usr/src/myapp
ENV PORT 8080
ENV REQUEST_ORIGIN http://localhost:5000
COPY . /usr/src/myapp
RUN go build
CMD [ "./server"]
