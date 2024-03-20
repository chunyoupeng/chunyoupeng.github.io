---
title: Docker Proxy Setting
date: 2023-03-18
author: Chunyou Peng
tags: ["tech"]
description: "docker settings"
type: "post"
---

# Docker Proxy

## Docker build

```sh
docker build --no-cache -t test:latest . \
--network host \
--build-arg HTTP_PROXY=http://127.0.0.1:7890 \
--build-arg HTTPS_PROXY=http://127.0.0.1:7890
```

> Note I add --no-cache flag

