FROM openjdk:8-jre-alpine


MAINTAINER "Saran Teja, Patnala" "v.n.v.saran.patnala@verizon.com"


RUN mkdir -p /app/application/logs/

# Add application jar
ADD target/poc_config.jar /app/application/poc_config.jar

RUN chmod 775 /app/application/poc_config.jar

RUN sh -c 'touch /app/application/poc_config.jar'

EXPOSE 8123



ENTRYPOINT ["java","-jar","/app/application/poc_config.jar"]