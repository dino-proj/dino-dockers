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

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## JDK:17
基于 `openjdk:17-jdk-slim`

```dockerfile

ENV IN_DOCKER=true

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## JDK:20
基于 `openjdk:20-jdk-slim`

```dockerfile

ENV IN_DOCKER=true

ENV APP_LOG_DIR=/logs

WORKDIR /app

ENTRYPOINT ["/bin/bash", "/app/bin/start", "--docker"]
```

## 📄 License

dino-dockers is an open source software licensed as [Apache-2.0](./LICENSE).
