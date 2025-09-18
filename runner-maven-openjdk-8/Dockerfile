FROM maven:3.8-openjdk-8-slim

COPY runner-maven-openjdk-8/settings.xml /usr/share/maven/conf/settings.xml

RUN apt-get update && apt-get install -y --no-install-recommends openssh-client && apt-get install zip unzip && rm -rf /var/lib/apt/lists/*

COPY config /root/.ssh/config
