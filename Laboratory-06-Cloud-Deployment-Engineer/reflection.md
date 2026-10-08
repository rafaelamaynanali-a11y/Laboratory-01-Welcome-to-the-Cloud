# Reflection

## 1. What was the most challenging part of deploying a multi-container application?

The most challenging part was understanding how the Nextcloud application and MariaDB database work together in separate containers. It was important to understand that the application container and database container have different roles. Using Docker Compose made the deployment easier because both services were defined in one configuration file and could be started together.

## 2. How does Docker Compose simplify multi-container deployments?

Docker Compose simplifies multi-container deployment by allowing multiple related services to be defined in a single `docker-compose.yml` file. Instead of creating and configuring each container separately, the required images, ports, and environment variables can be placed in the Compose file. The command `docker-compose up -d` can then start the services together, making the deployment more organized and easier to manage.

## 3. Why is it important to separate the application and database into different containers?

Separating the application and database into different containers helps organize the system into independent components. The Nextcloud application handles the web application, while MariaDB handles the database. This separation makes each component easier to manage, troubleshoot, update, and maintain without placing everything inside one container.

## 4. How does the application container know where the database is located?

The application container knows where the database is located through the `MYSQL_HOST=database` environment variable. The value `database` matches the name of the MariaDB service in the `docker-compose.yml` file. Because of this configuration, the Nextcloud application can communicate with the MariaDB database using the service name.

## 5. What skills did you gain from this activity?

This activity helped me improve my understanding of Docker containers, Docker Compose, and multi-container application deployment. I learned how to define services in a Compose file, configure environment variables, connect an application to a database container, and manage multiple services using Docker Compose commands. I also gained experience checking the status of containers, accessing the deployed Nextcloud application, and stopping the deployment when it was no longer needed.
