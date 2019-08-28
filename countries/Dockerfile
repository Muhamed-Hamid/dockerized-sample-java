FROM ubuntu:latest
RUN  apt-get update -y && \
     apt-get install default-jre -y && \
     mkdir /usr/src/countries

COPY  countries-assembly-1.0.1.jar /usr/src/countries/countries-assembly-1.0.1.jar
RUN  chmod +x /usr/src/countries
WORKDIR  /usr/src/countries
EXPOSE 8080
CMD  ["java", "-jar", "countries-assembly-1.0.1.jar"]
