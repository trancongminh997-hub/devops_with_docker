FROM golang:1.16
WORKDIR /usr/src/myapp
ARG request_origin=http://localhost:5000
ARG redis_host=redis
ARG postgres_host=postgres
ARG postgres_user=postgres
ARG postgres_password=postgres
ARG postgres_database=postgres
ENV PORT 8080
ENV REQUEST_ORIGIN=$request_origin
ENV REDIS_HOST=$redis_host
ENV POSTGRES_HOST=$postgres_host
ENV POSTGRES_USER=$postgres_user
ENV POSTGRES_PASSWORD=$postgres_password
ENV POSTGRES_DATABASE=$postgres_database
RUN curl -sL https://github.com/docker-hy/material-applications/archive/main.tar.gz | tar -xz --strip=2 material-applications-main/example-backend
RUN go build
CMD [ "./server"]
