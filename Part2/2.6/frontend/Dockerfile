FROM node:12
WORKDIR /usr/src/myapp
ARG react_app_backend_url=http://localhost:8080
ENV REACT_APP_BACKEND_URL=$react_app_backend_url
RUN curl -sL https://github.com/docker-hy/material-applications/archive/main.tar.gz | tar -xz --strip=2 material-applications-main/example-frontend
RUN npm install
RUN npm install -g serve
RUN npm run build
EXPOSE 5000
CMD serve -s -l 5000 build
