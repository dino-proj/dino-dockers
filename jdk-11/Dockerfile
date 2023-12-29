FROM openjdk:11-jdk-slim

LABEL org.opencontainers.image.authors="cody@dinodev.cn"

WORKDIR /app/

COPY ./bin/start /app/bin/

ENV IN_DOCKER=true

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]