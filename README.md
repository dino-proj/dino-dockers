<!--
 Copyright 2023 dinosdev.cn.
 SPDX-License-Identifier: Apache-2.0
-->

# 🦖 Dino Dockers
提供`Dino dev`所需的开发及运行环境的Docker images

## JDK:11
基于 `openjdk:11-jdk-slim`

```dockerfile

ENV IN_DOCKER=true

ENV JDK_VERSION=11

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## JDK:17
基于 `openjdk:17-jdk-slim`

```dockerfile

ENV IN_DOCKER=true

ENV JDK_VERSION=17

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## JDK:21
基于 `openjdk:21-jdk-slim`

```dockerfile

ENV IN_DOCKER=true

ENV JDK_VERSION=21

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## JDK:25
基于 `openjdk:25-jdk-slim`

```dockerfile

ENV IN_DOCKER=true

ENV JDK_VERSION=25

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## 📄 License

dino-dockers is an open source software licensed as [Apache-2.0](./LICENSE).
