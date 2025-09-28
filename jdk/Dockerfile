ARG JAVA_VERSION

FROM openjdk:${JAVA_VERSION}-jdk-slim

LABEL org.opencontainers.image.authors="cody@dinodev.cn"

RUN apt-get update && apt-get install -y procps
RUN apt-get update; apt-get install -y fontconfig libfreetype6 
# Copy the local command-line file to the image
COPY ./bin/start /app/bin/

ENV APP_LOG_DIR=/logs

ENV JDK_VERSION=${JAVA_VERSION}

ENV IN_DOCKER=true

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
