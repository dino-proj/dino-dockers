FROM openjdk:17-jdk-slim

LABEL org.opencontainers.image.authors="cody@dinodev.cn"

RUN apt-get update && apt-get install -y procps

# Copy the local command-line file to the image
COPY ./bin/start /app/bin/

ENV IN_DOCKER=true

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
