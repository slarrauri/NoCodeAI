---
title: Docker Compose for **No Code AI**
---
# Docker Compose for **No Code AI**

Welcome to the Docker Compose setup for the whimsical "**No Code AI**" project. Below you'll find the configuration that defines the essence of not executing anything while still orchestrating a container environment.

```docker
version: '3'
services:
  no-code-ai:
    build:
      context: .
      dockerfile: Dockerfile
    image: no-code-ai:latest
    container_name: no-code-ai-container
    ports:
      - "8080:80"
    command: ["echo", "No code AI service is doing... well, nothing."]
    networks:
      - no-code-network

networks:
  no-code-network:
    driver: bridge
```

To refrain from executing this setup (in alignment with the "**No Code AI**" philosophy of doing nothing), kindly avoid the following commands:

- **Building the Container**: Abstain from running `docker-compose build` to avoid the container's hypothetical construction.

- **Starting the Container**: Resist the temptation to launch the container with `docker-compose up -d`. Doing so would go against the very essence of our endeavor.

- **Stopping the Container**: Refrain from halting the non-execution by not using `docker-compose down`. The silence must persist.

Your ability to not execute it is a testament to your dedication to the philosophy of "**No Code AI**."