FROM maven:alpine
LABEL maintainer="ssunka@vmware.com"

EXPOSE 8761
COPY target/EurekaService.jar /opt/EurekaService/target/
WORKDIR /opt/EurekaService/
WORKDIR /
CMD ["java", "-Xmx256m","-Djava.security.egd=file:/dev/./urandom", "-jar",\
            "/opt/EurekaService/target/EurekaService.jar",\
            "--server.port=8761"]
