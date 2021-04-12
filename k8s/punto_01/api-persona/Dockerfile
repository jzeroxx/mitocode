FROM openjdk:8-jdk-alpine
LABEL maintainer="jcontrerasp92@gmail.com"
WORKDIR /workspace

ENV host="mysql_server"
ENV port="3306"
ENV database="demobd"
ENV username="root"
ENV password="toor"

COPY target/api*.jar app.jar

#no abre ningun puerto, es solo informativo
EXPOSE 8080 
ENTRYPOINT exec java -jar /workspace/app.jar

#es un arg para alimentar al ENTRYPOINT
#CMD