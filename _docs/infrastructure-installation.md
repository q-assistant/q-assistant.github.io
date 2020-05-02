---
title: Installation
subtitle: This document covers the initial setup
author: edwin
tags: [setup]
---

Requirements: 
- Docker [https://docs.docker.com/get-docker/][https://docs.docker.com/compose/install/]  
- Docker Compose [https://docs.docker.com/compose/install/][https://docs.docker.com/compose/install/]  

Download and unpack the infrastructure:

```bash
sudo mkdir /var/q && cd /var/q && \
wget -c "https://github.com/q-assistant/infrastructure/archive/v0.0.1-alpha0.tar.gz" -O - | sudo tar -xz && \
sudo mv infrastructure-0.0.1-alpha0 infrastructure && cd infrastructure && \
sudo cp graylog.env.dist graylog.env
```

Run the following command while you are in ```/var/q/infrastructure``` to start:
```bash
docker-compose up
// or detached
docker-compose up -d
```

After this you can go to [http://controller.localhost][http://controller.localhost] to continue setup.

[https://docs.docker.com/compose/install/]: https://docs.docker.com/get-docker/

[https://docs.docker.com/compose/install/]: https://docs.docker.com/compose/install/

[http://controller.localhost]: http://controller.localhost