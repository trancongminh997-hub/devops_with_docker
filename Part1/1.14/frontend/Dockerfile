FROM node:12
WORKDIR /usr/src/myapp
ENV REACT_APP_BACKEND_URL http://localhost:8080
COPY . /usr/src/myapp
RUN npm install
RUN npm install -g serve
RUN npm run build
EXPOSE 5000
CMD serve -s -l 5000 build
