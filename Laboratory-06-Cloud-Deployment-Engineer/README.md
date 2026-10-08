# Mission 6 – The Cloud Deployment Engineer

## Mission Overview

This mission focused on deploying a multi-container application using Docker Compose. The application consisted of a Nextcloud web application and a MariaDB database. Docker Compose was used to define, configure, start, and manage both services together.

The deployment demonstrated how a web application can communicate with a separate database container and how Docker Compose simplifies the management of related containers.

## Objectives

- Understand the concept of two-tier architecture.
- Deploy a multi-container application using Docker Compose.
- Configure a Nextcloud application container and a MariaDB database container.
- Understand how containers communicate with each other.
- Use environment variables to connect the application to the database.
- Practice starting and stopping multiple containers using Docker Compose.
- Document the deployment process and results.

## Commands Executed

### Start the Multi-Container Application

    docker-compose up -d

This command started the services defined in the `docker-compose.yml` file in detached mode.

### Check the Running Containers

    docker-compose ps

This command displayed the status of the services managed by Docker Compose.

### Stop and Remove the Containers

    docker-compose down

This command stopped and removed the containers created by Docker Compose.

## Skills Learned

Through this activity, I learned how to deploy and manage a multi-container application using Docker Compose. I learned how services are defined in a Compose file and how environment variables allow the application container to connect to the database container. I also gained experience using Docker Compose commands to start, check, and stop multiple services.

## Deployment Result

The deployment successfully started the Nextcloud application and MariaDB database services. The Nextcloud web interface was accessible through port 8080, demonstrating that the application container was running and communicating with the configured database service.

## Screenshots

The following screenshots document the deployment process:

- `screenshots/compose-deployment.png` – Docker Compose deployment and running containers.
- `screenshots/nextcloud-web.png` – Nextcloud web interface.
- `screenshots/compose-teardown.png` – Docker Compose teardown process.
