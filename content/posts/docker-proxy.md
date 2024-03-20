---
title: "Docker Proxy Settings"
author: Chunyou Peng
date: 2023-03-18
description: "Help with docker proxy"
tags: ["tech"]
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

