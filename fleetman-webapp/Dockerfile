FROM tomcat:8.5.47-jdk8-openjdk

MAINTAINER "Paula Bonastre"
EXPOSE 8080

RUN rm -rf /usr/local/tomcat/webapps/*

#Transfer or WAR file an start tomcat
COPY ./target/fleetman-0.0.1-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war

ENV JAVA_OPTS="-Dspring.profiles.active=docker-demo"

CMD ["catalina.sh", "run"]