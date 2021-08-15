FROM node:12
WORKDIR /usr/src/myapp
COPY . /usr/src/myapp
RUN npm install
RUN npm install -g serve
RUN npm run build
EXPOSE 5000
CMD serve -s -l 5000 build
