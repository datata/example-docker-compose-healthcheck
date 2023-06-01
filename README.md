# Example of Healthcheck with Docker Compose

This is an example of how to use Docker Compose to set up MySQL and Adminer containers implementing a healthcheck in your project.


To get started, clone the project and run the following command:

- If you have Docker version 1 installed, use the command 
```bash
docker-compose up
```

- If you have Docker version 2 installed, use the command 
```bash
docker compose up --wait
```

## What is a Healthcheck?

A healthcheck is a mechanism that allows you to verify the status of a running container. It can be used to ensure that the container is healthy and functioning properly.

## How to Implement a Healthcheck

To implement a healthcheck in your Docker Compose file, follow these steps:

1. Add a `healthcheck` section to the service definition in your `docker-compose.yml` file.
2. Specify the command or script that will be used to check the health of the container.
3. Set the `interval`, `timeout`, and `retries` parameters to control how often the healthcheck is performed and how long to wait for a response.
4. Optionally, you can set the `start_period` parameter to delay the healthcheck until a specific time after the container has started.
