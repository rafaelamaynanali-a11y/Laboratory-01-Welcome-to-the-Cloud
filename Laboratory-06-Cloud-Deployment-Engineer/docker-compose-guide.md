# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block in the `docker-compose.yml` file defines the containers that are part of the application.

In this laboratory activity, there are two services: `database` and `app`.

The `database` service runs the MariaDB database using the `mariadb:10.6` image. The `app` service runs the Nextcloud application using the `nextcloud` image.

By defining both services in the `services:` block, Docker Compose can manage the Nextcloud application and MariaDB database together.

## How Did the Nextcloud App Container Find the Database Container?

The Nextcloud application was configured with the environment variable `MYSQL_HOST=database`.

The value `database` is the name of the MariaDB service defined in the `services:` block.

The Nextcloud application also uses the following database settings:

    MYSQL_PASSWORD=cloudnova_pass
    MYSQL_DATABASE=nextcloud_db
    MYSQL_USER=nextcloud_user
    MYSQL_HOST=database

The `MYSQL_HOST=database` setting tells the Nextcloud application that the database it needs is available through the service named `database`.

Therefore, the Nextcloud app container can find and communicate with the MariaDB database container using the service name `database`.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is used to create and start a Docker container. It is commonly used when running a container individually.

For example:

    docker run <image>

The `docker-compose up -d` command is used to start the services defined in a `docker-compose.yml` file.

In this laboratory activity, the command used was:

    docker-compose up -d

This command started the services defined in the Compose file, including the Nextcloud application and MariaDB database.

The main difference is that `docker run` is generally used to run an individual container, while `docker-compose up -d` uses the configuration in the Compose file to deploy and manage multiple related services together.

The `-d` option runs the services in detached mode, allowing them to continue running in the background.
