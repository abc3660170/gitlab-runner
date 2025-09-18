FROM maven:3.9.4-eclipse-temurin-21-alpine

COPY runner-maven-openjdk-21/settings.xml /usr/share/maven/conf/settings.xml

RUN apk update

RUN apk add --no-cache openssh

RUN apk add --no-cache unzip zip

COPY config /root/.ssh/config
