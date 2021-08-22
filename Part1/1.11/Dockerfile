FROM openjdk:8
WORKDIR /myapp
RUN git clone https://github.com/docker-hy/material-applications.git
RUN cp -a material-applications/spring-example-project/. .
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar
EXPOSE 8080